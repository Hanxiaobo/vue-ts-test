<template>
  <div id="app">
    <HelloWorld msg="my first gh-page"/>
  </div>
</template>

<script lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import test from './test'
export default {
  name: 'App',
  components: {
    HelloWorld
  },
  mounted () {
    console.log(test)
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
