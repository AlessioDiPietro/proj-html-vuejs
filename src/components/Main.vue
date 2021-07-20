<template>
  <main>

    <!-- section Our Consultats -->
    <Consults/>

    <!-- section about us -->
    <AboutUs/>

    <!-- section project -->
    <Project :imgSlider="sliderImg"/>

    <!-- section Testimonial -->
    <Testimonial/>

    <!-- section blog -->
    <Blog/>

    
  </main>
</template>

<script>
import AboutUs from "@/components/AboutUs"
import Consults from "@/components/Consults"
import Project from "@/components/Project"
import Testimonial from "@/components/Testimonial"
import Blog from "@/components/Blog"
export default {
    name:"Main",
    components: {
      AboutUs,
      Consults,
      Project,
      Testimonial,
      Blog
    },
    props: ["sliderImg"]
}
</script>

<style>

</style>