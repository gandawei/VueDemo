<template>
  <div>
    <home-header></home-header>
    <header-title></header-title>
    <home-content></home-content>
    <home-footer></home-footer>
  </div>
</template>

<script>

 import HomeHeader from './components/header'
 import HeaderTitle from './components/title'
 import HomeContent from "./components/Content"
 import HomeFooter from './components/Footer'
 export default{
   name:'Home',
   components:{
     HomeHeader,HeaderTitle,HomeContent,HomeFooter
 },
 data () {
     return {
       swiperList: [],
       iconList: [],
       hotList: [],
       weekendList: []
     }
   },

}
</script>

<style>
</style>
