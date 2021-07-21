<template>
  <section>
    <div class="container-fluid py-3">
        <div class="row py-5 h_176 align-items-center">

            <div class="img_box w-25 pt-5">
                <img src="@/assets/images/logotype-2-300x50.png" alt="logo">
            </div>
              
            <NavBar class=" w-50"/>

            <div class="social_icon w-25 pt-5 text-end">
                <i class="fab fa-instagram"></i>
                <i class="fab fa-linkedin-in"></i>
                <i class="fab fa-facebook-f"></i>
                <i class="fab fa-twitter"></i>
            </div>
        </div>
        <hr>
        <div class="row py-5 justify-content-between ">
            <div class="tos col">
                <div>Terme Of Use</div>
                <div>Privacy Environmental Policy</div>
            </div>
            <div class="copyright col text-end align-self-end">
                <div>Copyright &#169; 2021 Phlox Consulting. All rights reserved.</div>
            </div>
        </div>
    </div>
  </section>
</template>

<script>
import NavBar from "@/components/NavBar.vue"
export default {
    name:"FooterInfo",
    components:{
        NavBar
    }

}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";
section{
    @include form_section_90;
    margin-top: 0;
    .h_176{
        height: 176px;
    }
    img{
        width:139px;
        height:23px
    }
    i {
        margin-left: 20px;
        font-size: 20px;
        cursor: pointer;
    }
    .tos, .copyright {
        color:$title_grey_txt;
    }
}
</style>