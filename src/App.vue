<template>
  <div id="app">

    <div class="container-fluid">
    <!-- intestazione +jb -->
    <Header/>

    <!-- corpo pagina + slider-->
    <Main/>

    <!-- info utili + anchor point -->
    <Footer/>

    </div> 

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import "@/assets/commons.scss";
@import "@/assets/ColorPhloxVar.scss";
#app {
  background-color: $blue_bg;
  // debug
  color: white;
}
</style>
