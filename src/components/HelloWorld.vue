<template>
  <new-contact></new-contact>
</template>

<script>
 import NewContact from './NewContact'
export default {
  name: 'HelloWorld',
  data () {    //由于是组件，data必须是个函数，这是ES6写法，data后面加括号相当于data: function () {}
    return {   //记得return不然接收不到数据
      msg: 'Welcome world' //上面的 msg 就是这里输出的
    }
  },
  components:{
    NewContact
}

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
a {
  color: #42b983;
}
</style>
