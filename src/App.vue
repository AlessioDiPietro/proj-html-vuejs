<template>
  <div id="app">

    <div class="container-fluid p-0">
    <!-- intestazione +jb -->
    <Header/>

    <!-- corpo pagina + slider-->
    <Main :sliderImg="imgSlider"/>

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
    Footer,
    
  },
  data(){
    return {
      imgSlider: [
        "DRY-1-790x592.jpg",
        "221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg",
        "z1el4c4p-790x592.jpg"
      ]
    }
  }
}
</script>

<style lang="scss">
@import "@/assets/commons.scss";
@import "@/assets/ColorPhloxVar.scss";
#app {
  background-color: $blue_bg;
  color: white;
    
  }
</style>
