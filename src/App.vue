<template>
  <div id="app">
    <img alt="Vue logo"
         src="./assets/logo.png">
    <div class="box"></div>
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.box {
  width: 100px;
  height: 100px;
  margin: auto;
  background: #7c7c7c;
}
.box::before {
  display: block;
  content: '';
  width: 20px;
  height: 20px;
  background: red;
}
</style>
