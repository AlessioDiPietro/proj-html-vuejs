<template>
  <header id="HOME">
      <div class="red_side position-relative">

        <div class="header_top d-flex justify-content-between">
            
            <img src="../assets/images/logotype.png" alt="logo">
            <NavBar/>
          
        </div>



        <div class="promo position-absolute">
            <div class="green_line"></div>
            <span>ALWATS THE BEST WAY YOU NEED IT</span>
            <h1>THE BEST BUSINESS CONSULTING</h1>
            <button>READ MORE</button>
            <button><i class="fas fa-play"></i></button>
        </div>

      </div>

  </header>
</template>

<script>
import NavBar from "@/components/NavBar.vue"
export default {
    name:"Header",
    components: {
        NavBar
    },
    

}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";
    .red_side {
        background-image: url("~@/assets/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg");
        background-repeat: no-repeat;
        background-position: right;
        height: 980px;
        .header_top{
            @include form_section_90;
            margin-top: 0;
        }
        .promo{
            width: 600px;
            left: 162px;
            top: 25%;
            font-size: 20px;
            .green_line {
                display: inline-block;
                height: 3px;
                width: 50px;
                margin-right: 20px;
                background-color: $opa_maringreen_bg;
            }
            h1 {
                font-size: 120px;
                font-weight:bolder;
            }
        }
    }
    img {
        width: 112px;
        height: 19px;
        margin-top: 43px;
        
    }

</style>