<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for ='item of swiperList' :key="item.id">
        <img class="swiper-img" :src="item.imgUrl" alt="">
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        loop: true,
        pagination: '.swiper-pagination'
      },
      swiperList: [
              {
                id: '001',
                imgUrl: 'https://img.18qweasd.com/d/file/html/gndy/jddyy/2019-09-03/95fc207da1adfc92eb704c0e75456a3f.jpg'
              },
              {
                id: '001',
                imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20191/61e0c45bd6f46af63f03fc19af63fd57.jpg_750x200_21f214c6.jpg'
              }
            ]
    }
  },

}
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background: #ffffff
  .wrapper
  overflow hidden
    width 100%
    height 0
    padding-bottom 31.25%
    .swiper-img
      min-height 2.5rem
      max-height 2.5rem
      width 100%
</style>
