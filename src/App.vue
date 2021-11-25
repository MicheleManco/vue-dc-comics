<template>
  <div id="app">
    <Header/>
    <Jumbo/>
    <Fumetti/>
    <Footer/>
  </div>
</template>

<script>
import Jumbo from './components/jumbo.vue'
import Header from './components/Headercomics.vue'
import Footer from './components/Footercomics.vue'
import Fumetti from './components/fumetti.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Fumetti,
    Jumbo
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
