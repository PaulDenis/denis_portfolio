<template>
  <div id="app">
    <Header />
    <NavBar @lingua="setLingua" />
    <Content />
    <Footer />
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
