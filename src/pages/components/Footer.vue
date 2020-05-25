<template>
  <div class="footer">
    <div>
      <ul>
        <li><a href="#"><div class="iconfont back-index">&#xe73d;</div></a></li>
        <li><a href="#"><div class="iconfont back-index">&#xe742;</div></a></li>
        <li><a href="#"><div class="iconfont back-index">&#xe749;</div></a></li>
        <li><a href="#"><div class="iconfont back-index">&#xe740;</div></a></li>
        <li><a href="#"><div class="iconfont back-index">&#xe743;</div></a></li>
      </ul>
     </div>
  </div>
</template>

<script>
  export default{
    name:'HomeFooter'
  }
</script>

<style lang="stylus" scoped>
  .footer
    background-color #F5F7FA
    height 50px
    line-height 50px
  .footer div
    width 100%
    margin 0 auto
  .footer div ul li
    display inline-block
    margin-right 0.21rem
  .footer div ul li a
    float left
    width 100%
    height 0.9rem
    margin auto 0.3rem
    text-align center
    border-radius 0.1rem
    color #F78989
  .footer div ul li a:active
    color #000000
  .back-index{
    font-size 0.5rem
    
  }
</style>
