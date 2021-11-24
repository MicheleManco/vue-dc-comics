<template>
  <div id="app">
    <Header/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Headercomics.vue'
import Footer from './components/Footercomics.vue'
import Main from './components/Maincomics.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Main
  }
}
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>
