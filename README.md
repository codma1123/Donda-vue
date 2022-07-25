# 🔁 돈다

> 재무제표 기반 주식가격 평가 서비스 프로젝트 **'돈다'** 의 웹 뷰 레포지토리 입니다.


## 개발 환경

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

  <br>

  <div align=center>    
    <img src="https://img.shields.io/badge/vue.js-4FC08D?&logo=vue.js&logoColor=white">  
    <img src="https://img.shields.io/badge/vue-2.6.14-green" />
  </div>

  프론트엔드 프레임워크 입니다. **Vuetify 2.6.0** 의 원활한 사용을 위해 Vue 2.6.0 버전을 채택하였습니다. 
  <u> **Vuetify**가 곧 3.0 버전 정식 릴리즈가 될 예정입니다. 릴리즈 내역에는 **Vue3.0** 이상 지원 내용이 포함되므로, **Vue 3.0** 으로 마이그레이션을 고려중입니다 다음 링크를 참조하세요.</u>
  > https://vuetifyjs.com/en/introduction/roadmap/#in-development

  <br>

  <div align=center>    
    <img src="https://img.shields.io/badge/typescript-3178C6?&logo=typescript&logoColor=white">    
  </div>

  복잡한 주가 데이터를 원활히 다루고, 백엔드와의 원활한 소통을 위해, 타입을 정의하고 사용하기 용이한 **Typescript**를 채택하였습니다.   

  <br>

  <div align=center>
    <img src="https://img.shields.io/badge/vuetify-1867C0?&logo=vuetify&logoColor=white">    
    <img src="https://img.shields.io/badge/vuetify-2.6.0-green">
  </div>

  **Vue.js** 의 **CSS** 프레임워크 입니다. **CSS** 요소를 간편하고 빠르게 만들기 위해 채택하였습니다.
  <u> **Vuetify**가 곧 3.0 버전 정식 릴리즈가 될 예정입니다. 릴리즈 내역에는 **Vue3.0** 이상 지원 내용이 포함됩니다.</u>
          



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





