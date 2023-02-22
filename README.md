# 🔁 **DONDA**

재무제표 기반 주식가격 평가 서비스 프로젝트 **DONDA** 의 웹 뷰 레포지토리 입니다.

<br/>
<br/>
<br/>
<div style="font-size:500%" align=center>
  🛠 Skills 
</div>


<div>
  <div align=center>
    <img src="https://img.shields.io/badge/vue.js-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white">
    <img src="https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white"> 
    <img src="https://img.shields.io/badge/html-E34F26?style=for-the-badge&logo=html5&logoColor=white"> 
    <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"> 
    <img src="https://img.shields.io/badge/vuetify-1867C0?style=for-the-badge&logo=vuetify&logoColor=white">       
  </div>

  <br>

  <div align=center>    
    <img src="https://img.shields.io/badge/vue-2.6.14-green">
    <img src="https://img.shields.io/badge/vuetify-2.6.0-green">
    <img src="https://img.shields.io/badge/vuex-3.6.2-green">
    <img src="https://img.shields.io/badge/vuexClass-0.3.2-blue">
    <img src="https://img.shields.io/badge/vuePropertyDecorator-9.1.2-blue">
    <img src="https://img.shields.io/badge/vueRouter-3.5.3-green">
    <img src="https://img.shields.io/badge/chart.js-2.9.4-green">
    <img src="https://img.shields.io/badge/axios-0.26.1-green">           
  </div>
</div>


<br/>
<br/>
<br/>
<div style="font-size:500%" align=center>
  🗂 Structure 
</div>
  
 <!-- ![GitHub top language](https://img.shields.io/github/languages/top/codma1123/Donda-vue?style=plastic)

 <!-- ![GitHub top language](https://img.shields.io/github/languages/second/codma1123/Donda-vue?style=plastic) -->
  
```bash
📦src
 ┣ 📂@types
 ┃ ┣ 📂chartjs-plugin-zoom
 ┃ ┃ ┗ 📜index.d.ts  
 ┃ ┗ 📜index.d.ts
 ┣ 📂api
 ┃ ┣ 📜stocks.ts
 ┃ ┗ 📜types.ts
 ┣ 📂assets
 ┃ ┣ 📜koreaflag.png
 ┃ ┣ 📜logo.png
 ┃ ┣ 📜logo.svg
 ┃ ┣ 📜readme-chart1.png
 ┃ ┣ 📜readme-chart2.png
 ┃ ┣ 📜readme-chart3.png
 ┃ ┗ 📜usaflag.png
 ┣ 📂mixins
 ┃ ┣ 📜DiviceMixin.vue
 ┃ ┣ 📜StockStoreMixin.vue
 ┃ ┣ 📜StoreMixin.vue
 ┃ ┣ 📜tools.ts
 ┃ ┗ 📜UserStoreMixin.vue
 ┣ 📂models
 ┃ ┣ 📜app.ts
 ┃ ┣ 📜interest.ts
 ┃ ┣ 📜market.ts
 ┃ ┣ 📜payload.ts
 ┃ ┣ 📜stock.ts
 ┃ ┗ 📜user.ts
 ┣ 📂plugins
 ┃ ┣ 📜directive.ts
 ┃ ┗ 📜vuetify.ts
 ┣ 📂routes
 ┃ ┗ 📜index.js
 ┣ 📂scss
 ┃ ┗ 📜variables.scss
 ┣ 📂store
 ┃ ┣ 📜index.ts
 ┃ ┣ 📜InterestStore.ts
 ┃ ┣ 📜MarketStore.ts
 ┃ ┣ 📜payload.ts
 ┃ ┣ 📜StockStore.ts
 ┃ ┣ 📜UserStore.ts
 ┃ ┗ 📜utils.ts
 ┣ 📂v2
 ┃ ┣ 📂components
 ┃ ┃ ┣ 📂detail
 ┃ ┃ ┃ ┣ 📂finance
 ┃ ┃ ┃ ┃ ┣ 📜FinanceContentFactory.vue
 ┃ ┃ ┃ ┃ ┣ 📜InformationFactory.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockFinance.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockFinanceBarChart.vue
 ┃ ┃ ┃ ┃ ┗ 📜StockFinanceLineChart.vue
 ┃ ┃ ┃ ┣ 📂indicator
 ┃ ┃ ┃ ┃ ┣ 📜IndicatorContentFactory.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockIndicator.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockIndicatorBarChart.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockIndicatorChart.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockIndicatorDetail.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockIndicatorLineChart.vue
 ┃ ┃ ┃ ┃ ┗ 📜StockPolarAreaChart.vue
 ┃ ┃ ┃ ┣ 📂similar
 ┃ ┃ ┃ ┃ ┣ 📜NewsContentsFactory.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockNews.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockSimiarContent.vue
 ┃ ┃ ┃ ┃ ┗ 📜StockSimilar.vue
 ┃ ┃ ┃ ┣ 📂stock
 ┃ ┃ ┃ ┃ ┣ 📜Stock.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockBigChart.vue
 ┃ ┃ ┃ ┃ ┗ 📜StockInfo.vue
 ┃ ┃ ┃ ┗ 📂valuation
 ┃ ┃ ┃ ┃ ┣ 📜StockScore.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockScoreBarChart.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockValuation.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockValuationChart.vue
 ┃ ┃ ┃ ┃ ┣ 📜StockValuationSingleChart.vue
 ┃ ┃ ┃ ┃ ┗ 📜ValuationBackgroundChart.vue
 ┃ ┃ ┣ 📂home
 ┃ ┃ ┃ ┣ 📜HomeNav.vue
 ┃ ┃ ┃ ┣ 📜MarketChart.vue
 ┃ ┃ ┃ ┣ 📜MarketTrend.vue
 ┃ ┃ ┃ ┣ 📜MarketTrendFactory.vue
 ┃ ┃ ┃ ┣ 📜MarketTrendLayout.vue
 ┃ ┃ ┃ ┣ 📜StockRecommend.vue
 ┃ ┃ ┃ ┗ 📜StockRecommendContent.vue
 ┃ ┃ ┣ 📂rank
 ┃ ┃ ┃ ┣ 📜RankComponent.vue
 ┃ ┃ ┃ ┗ 📜RankContents.vue
 ┃ ┃ ┗ 📂vuetify
 ┃ ┃ ┃ ┣ 📜BtnBadge.vue
 ┃ ┃ ┃ ┣ 📜BtnTooltip.vue
 ┃ ┃ ┃ ┗ 📜ProgressCircular.vue
 ┃ ┗ 📂pages
 ┃ ┃ ┣ 📜Detail.vue
 ┃ ┃ ┣ 📜Footer.vue
 ┃ ┃ ┣ 📜Home.vue
 ┃ ┃ ┣ 📜HomeCarousel.vue
 ┃ ┃ ┣ 📜NavBar.vue
 ┃ ┃ ┣ 📜NavBarMenus.vue
 ┃ ┃ ┣ 📜RankV2.vue
 ┃ ┃ ┣ 📜SearchBar.vue
 ┃ ┃ ┣ 📜SideBar.vue
 ┃ ┃ ┗ 📜SnackBar.vue
 ┣ 📜App.vue
 ┣ 📜main.ts
 ┣ 📜shims-tsx.d.ts
 ┣ 📜shims-vue.d.ts
 ┗ 📜shims-vuetify.d.ts

📂@types      - ts로 재정의한 npm 라이브러리를 담고 있습니다.
📂api         - api url과 요청 타입을 담고있습니다.
📂assets      - 외부 파일을 담습니다.
📂components  - 페이지에 그려질 컴포넌트들을 담고 있습니다. 
📂mixins      - Vue의 mixins과 각종 유틸 함수들을 담고 있습니다.      
📂models      - 각종 데이터 모델을 정의합니다.
📂pages       - 페이지를 담고 있습니다.
📂plugins     - Vue의 plugins을 정의합니다.
📂routes      - 라우트 설정을 정의합니다.
📂store       - vuex store들을 정의합니다.

📂components
 ┣ 📂detail    - 디테일 페이지에 필요한 컴포넌트들을 담고 있습니다.
 ┣ 📂home      - 홈 페이지에 필요한 컴포넌트들을 담고 있습니다.
 ┣ 📂rank      - 랭크 페이지에 필요한 컴포넌트들을 담고 있습니다.

```
## 컴포넌트

## API

**돈다** 웹 뷰에서 API 요청은 **📦src/📂store** 에서 **Vuex**의 **@Action** 데코레이터로써 정의됩니다. <br>
**종목 하나의 정보** 를 가져오는  **getStock** 함수를 예시를 통해 알아봅시다.

**📦src/📂store/📜StockStoreV2.ts**
```js
  @Action
  public async getStock(name: string): Promise<void> {
    try {
      this.context.commit('updateState', {
        stockLoaded: true
      })

      const res = await axios.get(`/stock/${name}`, HEADER)

      this.context.commit('updateState', {
        stock: res.data,
        stockLoaded: false
      })
    } catch(e) {
      console.log(e)
    }
  }  
```

```js
  this.context.commit('updateState', {
    stockLoaded: true
  })
```

먼저, *context** 객체의 *commit** 함수를 호출합니다. 첫번째 인자로는 *Mutation** 이름, 두번째 인자는 첫번째 인자에 명시된 Mutation 의 인자로써 사용됩니다. 여기서는 **updateState**의 인자로써 **{ stockLoaded: true }** 를 보내어 호출합니다. <br>

> ***context**** : 현재 store의 메소드와 객체들을 가지고 있는 객체입니다.<br>
> ***commit**** : 현재 store의 *Mutation* 을 호출합니다. </br>
> ***Mutation**** : vuex의 store의 *state** 를 변경하는 동기적 함수들을 의미합니다. </br>
> ***state**** : 접근이 허용된 컴포넌트에서 공통적으로 사용 가능한 store의 변수들을 의미합니다. <br>

<br>


```js
  @Mutation
  public updateState(payload: IUpdateStateModel) {    
    Object.entries(payload).forEach(state => {
      this[state[0]] = state[1]
    })        
  }
```
**updateState** Mutation은 다음과 같이 정의되어 있습니다. 인자로받은 payload의 **key**값에 해당하는 **state**를 **value**값으로 대체합니다.

<br>

```js
  this.context.commit('updateState', {
    stockLoaded: true
  })
```
따라서, 해당 구문은 ***stockLoaded**** 라는 **state**값을 **true**로 변경한다는 의미가 됩니다.
> ***stockLoaded**** : 종목 하나의 정보를 가져오는 중임을 의미하는 로딩 변수입니다. true면 종목을 정보를 로딩하는중, false면 정보를 로딩 완료했다는 뜻입니다. 이 state는 로딩 화면을 시각화 할때 사용됩니다.

<br>

```js
  const res = await axios.get(`/stock/${name}`, HEADER)
```
로딩 변수를 true로 변경한 후, axios get 요청을 실행합니다. axios의 get 함수에서 첫번째 인자는 요청할 url을 의미합니다. 두번째 인자는 http 헤더를 의미합니다.
> **돈다** 에서 사용되는 전체 API 요청은 [해당 링크](https://github.com/cd-hk-money/stock-server)에서 확인하실 수 있습니다. 

<br>

```js
  this.context.commit('updateState', {
    stock: res.data,
    stockLoaded: false
  })
```

그 후, 다시 *context* 객체의 *commit* 함수를 호출합니다. 호출할 Mutation은 updateState입니다.

### 결과적으로 **stock** 이라는 종목 정보들을 담는 **state** 에 axios 요청으로 받은 응답 객체의 **data** 값이 들어가게 됩니다.


## 차트

<div align=center>

  ![readme-chart3](https://user-images.githubusercontent.com/82079706/181083053-9960d3be-ceb4-4388-bd55-abd1f30d8206.png)
  
  ![readme-chart1](https://user-images.githubusercontent.com/82079706/181082442-32fbc64f-197a-4d5c-a053-5f707a929a72.png)

  ![readme-chart2](https://user-images.githubusercontent.com/82079706/181082802-7a15d6bf-28bf-4fc0-9430-7ff2bf37ab44.png)


</div>

차트는 **돈다** 에서 가장 중요한 요소 중 하나입니다. <br>
**돈다** 에서 차트는 **chart.js** 라이브러리와 CSS를 사용하여 구현되었습니다.




