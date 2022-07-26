<template>
  <v-card 
    :class="['ml-5', mobile ? 'stock-info-mobile' : 'mt-5']"    
    :height="mobile ? 240 : 240"
    width="94%"
    outlined   
    elevation="0"    
  >    
    <template v-if="!loaded">
      <v-list-item three-line>  
        <v-list-item-content>
          <div class="mb-4">
            {{ stock.market }} 
          </div>
          <v-list-item-title class="text-h4 font-weight-bold m-1 ml-5">
            <span>{{ stock.name }}</span>                        
            <v-tooltip right>
              <template v-slot:activator="{on}">
                <v-icon v-on="on" size="30" class="ml-5" color="red">fa-solid fa-arrow-trend-up</v-icon>
              </template>
              <span class="red--text font-weight-bold">상승</span> 
              <span> 추세입니다.</span>
            </v-tooltip>
          </v-list-item-title>
          <v-list-item-subtitle class="text-h5 mb-1 ml-6">
            {{ stock.code }}
          </v-list-item-subtitle>
        </v-list-item-content>
  
        <v-list-item-avatar>                  
          <v-dialog
            v-model="dialog"
            width="auto"
            height="auto"
          >
            <template v-slot:activator="{ on, attrs }">
              <v-btn icon x-large
                v-on="on"
                @click="bookmarked ? removeBookmarking : null"
                v-bind="attrs"
              >
                <v-icon size="40">{{ bookmarked ? 'mdi-bookmark' : 'mdi-bookmark-outline' }}</v-icon>
              </v-btn>
            </template>
  
            <v-card>
              <v-card-title class="text-h5">
                관심 종목 추가
              </v-card-title>
  
              <v-card-text>
                어느 그룹에 추가하시겠습니까?
              </v-card-text>
  
              <v-divider></v-divider>
            
              <v-list>                  
                <v-list-item 
                  :key="group.title"
                  v-for="group in interestGroups"
                  @click="activeBookmarking(group, stock)"
                >
                  <v-list-item-content>
                    <v-list-item-title class="ml-2">
                      {{ group.title }}
                    </v-list-item-title>
                  </v-list-item-content>
                </v-list-item>
              </v-list>
              
              <v-divider></v-divider>
  
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn
                  color="primary"
                  text
                  @click="dialog = false"
                >
                  확인
                </v-btn>
              </v-card-actions>              
            </v-card>
          </v-dialog>
        </v-list-item-avatar>              
  
      </v-list-item>
  
      <v-sheet 
        elevation="0"
        outlined        
        height="120"
      >                
        <v-card-title class="text-h5 font-weight-bold ml-5">
          <span>{{ stock.close.toLocaleString()}} ₩</span>
          <v-btn  
            class="ml-3"
            icon
            right
            x-small
          ><v-icon>fa-solid fa-circle-info</v-icon>
          </v-btn>
        </v-card-title>

        <v-card-subtitle :class="['text-h6', 'font-weight-bold', 'ml-5', stock.changes > 0 ? 'red--text' : 'blue--text']">
          <span>{{ stock.changes > 0 ? '+' + stock.changes : stock.changes }}₩ ({{ stock.changes_ratio > 0 ? '+' + stock.changes_ratio : stock.changes_ratio}}%)</span>                        
        </v-card-subtitle>
        
        <div class="stock-info-date">
          {{ stock.date }}
        </div>
      </v-sheet>
    </template>
    <template v-else>
      <div class="text-center stockinfo-progress-circular">
        <v-progress-circular
          indeterminate
          color="#40E0D0"
        ></v-progress-circular>
      </div>

    </template>

    <!-- Delete SparkLine -->
  </v-card>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import { namespace } from 'vuex-class'

import { IStockModel } from '@/models/stock'
import { IInterestGroup, IInterestGroupItem } from '@/models/interest'
import { mobileHeight } from '@/mixins/tools'

const StockStoreModule = namespace('StockStore')
const InterestStoreModule = namespace('InterestStore')

@Component
export default class StockInfo extends Vue {


  // datas
  dialog = false
  bookmarked = false
  
  // StockStore
  @StockStoreModule.State('stock') stock!: IStockModel
  @StockStoreModule.State('stockLoaded') loaded!: boolean
  @StockStoreModule.Action('getStock') getStock!: (name: string) => Promise<void>

  // InterestStore
  @InterestStoreModule.State('interestGroups') interestGroups!: IInterestGroup[]
  @InterestStoreModule.State('snackBar') snackBar!: boolean
  @InterestStoreModule.Mutation('snackBarOpen') snackBarOpen!: () => void
  @InterestStoreModule.Mutation('addInterestGroupItem') addInterestGroupItem!: (payload: {title: string, item: IInterestGroupItem}) => void
  @InterestStoreModule.Mutation('initInterestGroup') readonly initInterestGroup!: () => void
  @InterestStoreModule.Mutation('removeInterestGroupItem') removeInterestGroupItem!: (itemTitle: string) => void

  activeBookmarking (group: IInterestGroup, stock: IStockModel): void {
    this.addInterestGroupItem({
      title: group.title,
      item: {
        title: stock.name,
        code: stock.code
      }
    })

    this.dialog = false
    this.bookmarked = true    
    this.snackBarOpen()
  }

  removeBookmarking () {    
    this.bookmarked = false
    this.removeInterestGroupItem(this.stock.name)
  }

  get mobile () {
    return mobileHeight(this.$vuetify.breakpoint.name) < 500
  }
      
  async created () {    
    await this.getStock(this.$route.params.title)
    console.log(this.stock)
  }  
}
</script>
<style scoped>
.stockinfo-progress-circular {
  top: 50%;
  left: 50%;
  right: 50%;
  position: absolute;
}

.stock-info-mobile {
  margin-top: 75px;
}

.stock-info-date {
  position: absolute;
  bottom: -5px;
  right: 13px;
  opacity: .5;
}
</style>