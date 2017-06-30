<template>
  <div id="app">
    <h1 class="">Grzegorz Hadała</h1>
    <h3>Product Designer</h3>
    <router-view></router-view>
  </div>
</template>

<script>
import '../node_modules/mini.css/dist/mini-default.min.css'
import Hello from '@/components/Hello'
export default {
  name: 'app',
  components: {
    Hello
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  padding: 5em;
}
</style>
