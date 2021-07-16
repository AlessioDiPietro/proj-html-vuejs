<template>
  <main>

    <!-- section Our Consultats -->
    <Consults/>

    <!-- section project -->
    <Project/>

    <!-- section Testimonial -->
    <Testimonial/>

    <!-- section blog -->
    <Blog/>

    
  </main>
</template>

<script>
import Consults from "@/components/Consults"
import Project from "@/components/Project"
import Testimonial from "@/components/Testimonial"
import Blog from "@/components/Blog"
export default {
    name:"Main",
    components: {
      Consults,
      Project,
      Testimonial,
      Blog
    }
}
</script>

<style>

</style>