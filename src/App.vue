<template>
  <div id="app">
    <h1 class="">Grzegorz Hadała</h1>
    <h3>Product Designer</h3>
    <transition name="fade">
      <router-view></router-view>
    </transition>
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
.fade-enter-active, .fade-leave-active {
  transition: All .5s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active in <2.1.8 */ {
  opacity: 0;
  position: absolute;
  top: 0;
}
</style>
