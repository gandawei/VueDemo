<template>

  <div class="content" >
    <vue-scroll :ops="ops">
      <div class="content-item" v-for="item of dataList" v-bind:key="item.id">
        <div v-if="item.image" class="contentimage">
          <div class="left">
            <div class="contentimage-title">
              <a href="#">{{item.title}}</a>
            </div>
            <div class="contentimage-info">{{item.source}}</div>
          </div>
          <div class="right">
            <img v-bind:src='item.imgUrl'/>
          </div>
        </div>
        <div v-else class="contentnoimage">
        <div class="contentnoimage-title">
        <a href="#">{{item.title}}</a>
        </div>
        <div class="contentnoimage-info">{{item.source}}</div>
      </div>
    </div>
    </vue-scroll>
  </div>

</template>

<script>
  export default{
    name:"HomeContent",
    data () {
      return {
        dataList: [
                {
                  id: '001',
                  image:true,
                  imgUrl: require('@/assets/1.jpg'),
                  title:'第一条新闻不晓得些什么',
                  source:'政府新媒体',
                },
                {
                  id: '002',
                  image:false,
                  imgUrl: 'https://img.18qweasd.com/d/file/html/gndy/jddyy/2019-09-03/95fc207da1adfc92eb704c0e75456a3f.jpg',
                  title:'第二条新闻搞不清些什么，你知道吗爱不晓得怎么高哦',
                  source:'CCTV',
                },
                {
                  id: '003',
                  image:true,
                  imgUrl: 'https://img.18qweasd.com/d/file/html/gndy/jddyy/2019-09-03/95fc207da1adfc92eb704c0e75456a3f.jpg',
                  title:'第二条新闻搞不清些什么，你知道吗爱不晓得怎么高哦',
                  source:'CCTV',
                },
                {
                  id: '003',
                  image:true,
                  imgUrl: 'https://img.18qweasd.com/d/file/html/gndy/jddyy/2019-09-03/95fc207da1adfc92eb704c0e75456a3f.jpg',
                  title:'第二条新闻搞不清些什么，你知道吗爱不晓得怎么高哦',
                  source:'CCTV',
                },
                {
                  id: '003',
                  image:true,
                  imgUrl: 'https://img.18qweasd.com/d/file/html/gndy/jddyy/2019-09-03/95fc207da1adfc92eb704c0e75456a3f.jpg',
                  title:'第二条新闻搞不清些什么，你知道吗爱不晓得怎么高哦',
                  source:'CCTV',
                },
                {
                  id: '003',
                  image:true,
                  imgUrl: 'https://img.18qweasd.com/d/file/html/gndy/jddyy/2019-09-03/95fc207da1adfc92eb704c0e75456a3f.jpg',
                  title:'第二条新闻搞不清些什么，你知道吗爱不晓得怎么高哦',
                  source:'CCTV',
                },
                {
                  id: '003',
                  image:true,
                  imgUrl: 'https://img.18qweasd.com/d/file/html/gndy/jddyy/2019-09-03/95fc207da1adfc92eb704c0e75456a3f.jpg',
                  title:'第二条新闻搞不清些什么，你知道吗爱不晓得怎么高哦',
                  source:'CCTV',
                },
                {
                  id: '003',
                  image:true,
                  imgUrl: 'https://img.18qweasd.com/d/file/html/gndy/jddyy/2019-09-03/95fc207da1adfc92eb704c0e75456a3f.jpg',
                  title:'第二条新闻搞不清些什么，你知道吗爱不晓得怎么高哦',
                  source:'CCTV',
                },
                {
                  id: '003',
                  image:true,
                  imgUrl: 'https://img.18qweasd.com/d/file/html/gndy/jddyy/2019-09-03/95fc207da1adfc92eb704c0e75456a3f.jpg',
                  title:'第二条新闻搞不清些什么，你知道吗爱不晓得怎么高哦',
                  source:'CCTV',
                },
                {
                  id: '003',
                  image:true,
                  imgUrl: 'https://img.18qweasd.com/d/file/html/gndy/jddyy/2019-09-03/95fc207da1adfc92eb704c0e75456a3f.jpg',
                  title:'第二条新闻搞不清些什么，你知道吗爱不晓得怎么高哦',
                  source:'CCTV',
                },
              ],
        ops: {
              vuescroll: {},
              scrollPanel: {},
              rail: {},
              bar: {
                showDelay: 500,
                onlyShowBarOnScroll: true,
                keepShow: false,
                background: "#01a99a",
                opacity: 1,
                hoverStyle: false,
                specifyBorderRadius: false,
                minSize: 0.9,
                size: '3px',
                disable: false,
              },

              }
      }
    },
  }
</script>

<style lang="stylus" scoped>
  .content
    width:100%;
    height:545px;
    overflow-y true
  .content .content-item
    display flex
    padding 0.10rem 0rem
    margin 0 0.2rem
    border-bottom 0.1px solid #A6A9AD
  .contentimage{
    width 100%
  }
  .content .content-item .contentimage .left
    width 63%
    float left
    padding 0.1rem 0rem

  .content .content-item .contentimage .left .contentimage-title
    font-size 0.3rem
    font-weight 600
    line-height 0.4rem
    letter-spacing 0.005rem
    overflow hidden
   .contentimage-title a
     color #000000
   .contentimage-title a:hover
     cursor pointer
   .contentimage-title a:active
    color #606266

  .content .content-item .contentimage .left .contentimage-info
    margin-top 0.2rem
    font-size 0.2rem
    color #72767B

  .content .content-item .contentimage .right
    float left
    height 1.4rem
    width 30%
    margin-left 0.2rem
    padding 0.2rem auto
  .right img
     width: auto;
     height: auto;
     max-width: 100%;
     max-height: 100%;
     border-radius 0.2rem
  .contentnoimage
    margin 0.1rem 0
    padding 0.15rem 0rem
  .contentnoimage-title
    font-size 0.3rem
    font-weight 600
    line-height 0.4rem
    letter-spacing 0.005rem
   .contentnoimage-title a
     color #000000
   .contentnoimage-title a:hover
     cursor pointer
   .contentnoimage-title a:active
    color #606266
   .contentnoimage-info
    margin-top 0.25rem
    font-size 0.2rem
    color #72767B

</style>
