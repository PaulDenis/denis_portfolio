<template>
  <div id="app">
    <Header :lingua="lingua"/>
    <NavBar @lingua="setLingua" />
    <Content :lingua="lingua"/>
    <Footer :lingua="lingua"/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import NavBar from './components/NavBar.vue'
import Content from './components/Content.vue'
import Footer from './components/Footer.vue'
export default {
  name: 'App',
  components: {
    Header,
    NavBar,
    Content,
    Footer
  },
  data() {
    return {
      lingua:"american english"
    }
  },
  methods: {
    setLingua: function(lingua) {
      // console.log(lingua)
      return this.lingua = lingua;
    }
  }
}
</script>

<style lang="scss">
  @import './style/common'; 
</style>
