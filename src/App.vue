<template>
  <div id="app">
    <Header />
    <NavBar />
    <Content />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import NavBar from './components/NavBar.vue'
import Content from './components/Content.vue'
export default {
  name: 'App',
  components: {
    Header,
    NavBar,
    Content
  }
}
</script>

<style lang="scss">
  @import './style/common'; 
</style>
