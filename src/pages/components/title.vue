<template>
  <div class="title">
    <ul>
      <li><a href="#">今天</a></li>
      <li><a href="#">明天</a></li>
      <li><a href="#">后天</a></li>
      <li><a href="#">大后天</a></li>
    </ul>
  </div>
</template>

<script>
export default{
  name:"HeaderTitle"
}
</script>

<style lang="stylus" scoped>
.title
  height:0.6rem;
  line-height:0.6rem;
  font-size 0.25rem;
  display:flex;
  background: $bgColor;
  border-bottom 0.0008rem solid #82848A;
  color #000000;
.title ul{
  list-style none;
}
.title ul li{
  float left;
  margin:auto 0.1rem;
}
.title ul li a{
  text-decoration:none;
  color:#000000;
  padding 0.08rem 0.2rem;
}
</style>
