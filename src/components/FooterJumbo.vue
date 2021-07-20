<template>
  <section class="p-5">
      <div class="container-fluidc p-5">
          <div class="box_content p-5 text-center">
              <h2>LET'S TALK ABOUT WORK</h2>
              <p class="my-3">A wonderful serenity has taken possession Far far away, behind the word mountains.</p>
              <button>GET STARTED</button>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name:"FooterJumbo"
}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";
section {
    background-image: url("../assets/images/business-people-working-together-on-project-and-B3MZ4TX.jpg");
    .box_content{
        h2{
            @include title_sec_name;
        }
        p{
            color: $parag_grey_txt;
            width: 30%;
            margin: auto;
            font-size: 19px;
        }
        button{
            color: $title_grey_txt
        }
    }
    
}

</style>