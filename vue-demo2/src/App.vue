<template>
  <div class="app">
    我是一个app组件
    <h1>{{ msg }}</h1>
    <button class="btn">按钮1</button>
    <Hello></Hello>
  </div>
</template>

<script>
import Hello from './components/Hello.vue'
export default {
  data: function() {
    return {
      msg: '张三'
    }
  },
  components: {
    Hello: Hello
  }
}
</script>

<style lang='scss' scoped>
body {
  background: red;
}
.app {
  h1 {
    color: blue;
  }
}
.btn {
  background: green
}

</style>
