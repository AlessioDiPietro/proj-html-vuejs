<template>
  <section class="p-5" id="CONTACT">
      <div class="container-fluid p-5">
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
    background-size: cover;
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
            @include btn_blue;
            &:hover{
            animation: colorbtn 1s ease 0s 1 normal forwards;
                @keyframes colorbtn {
                    0% {
                        animation-timing-function: ease-in;
                        opacity: 0;
                        transform: scale(7);
                    }

                    38% {
                        animation-timing-function: ease-out;
                        opacity: 1;
                        transform: scale(1);
                    }

                    55% {
                        animation-timing-function: ease-in;
                        transform: scale(1.5);
                    }

                    72% {
                        animation-timing-function: ease-out;
                        transform: scale(1);
                    }

                    81% {
                        animation-timing-function: ease-in;
                        transform: scale(1.24);
                    }

                    89% {
                        animation-timing-function: ease-out;
                        transform: scale(1);
                    }

                    95% {
                        animation-timing-function: ease-in;
                        transform: scale(1.04);
                    }

                    100% {
                        animation-timing-function: ease-out;
                        transform: scale(1);
                        background-color: $int_maringreen_bg;
                    }
                }    
            } 
        }
    }
    
}

</style>