<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld :coords="coords" :typemap="typemap" :zoom="zoom" :size="size"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data(){
    return {
      coords:[55.88,37.77],
      typemap:'sat,skl',
      zoom:10,
      size:[480,320],
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
