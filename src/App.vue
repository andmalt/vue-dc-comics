<template>
  <div id="app">
    <Header/>
    <Jumbotron/>
    <Main/>
    <Pane/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbotron from './components/Jumbotron.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import Pane from './components/PaneMenu.vue'

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Main,
    Pane,
    Footer,
  }
}
</script>

<style lang="scss">
@import "./style/variables.scss";

*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>
