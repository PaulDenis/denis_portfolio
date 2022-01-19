<template>
  <div id="app">
    <Header />
    <NavBar />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import NavBar from './components/NavBar.vue'
export default {
  name: 'App',
  components: {
    Header,
    NavBar
  }
}
</script>

<style lang="scss">
  @import './style/common'; 
</style>
