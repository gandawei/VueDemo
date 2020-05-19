<template>
  <div>
    <home-header></home-header>
    <home-swiper :swiperList="swiperList"></home-swiper>

  </div>
</template>

<script>

 import HomeHeader from './components/header'
 import HomeSwiper from './components/swiper'
 export default{
   name:'Home',
   components:{
     HomeHeader,HomeSwiper
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
