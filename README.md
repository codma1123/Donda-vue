# 🔁 돈다

## 개발 환경

<div align=center>
  <img src="https://img.shields.io/badge/vue.js-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white">  
  <img src="https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white"> 
  <img src="https://img.shields.io/badge/html-E34F26?style=for-the-badge&logo=html5&logoColor=white"> 
  <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"> 
  <img src="https://img.shields.io/badge/vuetify-1867C0?style=for-the-badge&logo=vuetify&logoColor=white">       
</div>


<br><br/>
 <!-- ![GitHub top language](https://img.shields.io/github/languages/top/codma1123/Donda-vue?style=plastic)

 ![GitHub top language](https://img.shields.io/github/languages/second/codma1123/Donda-vue?style=plastic) -->

 



```bash
📦src
 ┣ 📂@types
 ┃ ┣ 📂chartjs-plugin-zoom
 ┃ ┃ ┗ 📜index.d.ts
 ┃ ┣ 📂vue-mobile-detection
 ┃ ┃ ┗ 📜index.d.ts
 ┃ ┗ 📜index.d.ts
 ┣ 📂assets
 ┃ ┣ 📜logo.png
 ┃ ┗ 📜logo.svg
 ┣ 📂mixins
 ┃ ┣ 📜tools.ts
 ┃ ┗ 📜TopListMixin.vue
 ┣ 📂models
 ┃ ┣ 📜app.ts
 ┃ ┣ 📜interest.ts
 ┃ ┣ 📜market.ts
 ┃ ┣ 📜payload.ts
 ┃ ┣ 📜stock.ts
 ┃ ┗ 📜user.ts
 ┣ 📂plugins
 ┃ ┗ 📜vuetify.ts
 ┣ 📂routes
 ┃ ┗ 📜index.js
 ┣ 📂scss
 ┃ ┗ 📜variables.scss
 ┣ 📂store
 ┃ ┣ 📜index.ts
 ┃ ┣ 📜InterestStore.ts
 ┃ ┣ 📜MarketStore.ts
 ┃ ┣ 📜StockStore.ts
 ┃ ┣ 📜StockStoreV2.ts
 ┃ ┗ 📜UserStore.ts
 ┣ 📂v2
 ┃ ┣ 📂components
 ┃ ┃ ┣ 📂detail
 ┃ ┃ ┃ ┣ 📜Stock.vue
 ┃ ┃ ┃ ┣ 📜StockBigChart.vue
 ┃ ┃ ┃ ┣ 📜StockChart.vue
 ┃ ┃ ┃ ┣ 📜StockDrawer.vue
 ┃ ┃ ┃ ┣ 📜StockFinance.vue
 ┃ ┃ ┃ ┣ 📜StockFinanceBarChart.vue
 ┃ ┃ ┃ ┣ 📜StockFinanceLineChart.vue
 ┃ ┃ ┃ ┣ 📜StockIndicator.vue
 ┃ ┃ ┃ ┣ 📜StockIndicatorBarChart.vue
 ┃ ┃ ┃ ┣ 📜StockIndicatorChart.vue
 ┃ ┃ ┃ ┣ 📜StockInfo.vue
 ┃ ┃ ┃ ┣ 📜StockMarcapChart.vue
 ┃ ┃ ┃ ┣ 📜StockNews.vue
 ┃ ┃ ┃ ┣ 📜StockScore.vue
 ┃ ┃ ┃ ┣ 📜StockScoreBarChart.vue
 ┃ ┃ ┃ ┣ 📜StockSimilar.vue
 ┃ ┃ ┃ ┣ 📜StockSimilarContents.vue
 ┃ ┃ ┃ ┣ 📜StockValuation.vue
 ┃ ┃ ┃ ┗ 📜StockValuationChart.vue
 ┃ ┃ ┣ 📂home
 ┃ ┃ ┃ ┣ 📜Market.vue
 ┃ ┃ ┃ ┣ 📜MarketChart.vue
 ┃ ┃ ┃ ┣ 📜MarketDesc.vue
 ┃ ┃ ┃ ┣ 📜MarketTrend.vue
 ┃ ┃ ┃ ┗ 📜StockRecommend.vue
 ┃ ┃ ┗ 📂rank
 ┃ ┃ ┃ ┣ 📜RankComponent.vue
 ┃ ┃ ┃ ┗ 📜RankContents.vue
 ┃ ┗ 📂pages
 ┃ ┃ ┣ 📜AppBar.vue
 ┃ ┃ ┣ 📜DetailV2.vue
 ┃ ┃ ┣ 📜HomeV2.vue
 ┃ ┃ ┣ 📜InterestToggle.vue
 ┃ ┃ ┣ 📜MenuBar.vue
 ┃ ┃ ┣ 📜RankV2.vue
 ┃ ┃ ┗ 📜SideBar.vue
 ┣ 📜App.vue
 ┣ 📜main.ts
 ┣ 📜shims-tsx.d.ts
 ┣ 📜shims-vue.d.ts
 ┗ 📜shims-vuetify.d.ts

📂assets      - 앱에 필요한 외부 파일을 담습니다.
📂components  - 레이아웃에 그려질 컴포넌트들을 담습니다. 
📂layout      - 페이지에 그려질 레이아웃을 담습니다.      
📂mixins      - Vue의 mixins들을 담습니다.      
📂models      - 각종 데이터 모델을 정의합니다.
📂pages       - 페이지들을 담습니다.
📂plugins     - Vue의 각종 plugins을 정의합니다.
📂routes      - 라우트 설정을 정의합니다.
📂store       - vuex store들을 정의합니다.

```


