<template>
  <div id="app">
    <nav-bar v-if="$route.meta.isNavBar"></nav-bar>
    <router-view></router-view>
  </div>
</template>

<script>
import navBar from '@/components/navBar'

export default {
  name: 'App',
  components: {
    navBar
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
  height: 100vh;
}
</style>
