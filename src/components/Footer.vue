<template>
  <footer>
    <FooterJumbo/>

    <FooterInfo/>
  </footer>
</template>

<script>
import FooterJumbo from "@/components/FooterJumbo.vue"
import FooterInfo from "@/components/FooterInfo.vue"
export default {
    name:"Footer",
    components:{
      FooterJumbo,
      FooterInfo
    }
}
</script>

<style>

</style>