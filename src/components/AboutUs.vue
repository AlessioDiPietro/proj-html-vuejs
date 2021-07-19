<template>
  <section>
    <div class="container-fluid p-0">
        <div class="row w-100">

            <div class="left_side col">
              <img src="@/assets/images/business-people-working-together-on-project-and-5FHSKBL.jpg" alt="Consulting People">
            </div>

            <div class="right_side col px-5 d-flex align-items-center">
              <div class="box_text w-75">
                <div class="line_titles "></div>
                <span>ABOUT US</span>
                <h2>WE MAKE YOUR STRATEGY WORK</h2>
                <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed when I hear the buzz of the little world among the stalks,and grow familiar indescribable forms of the insects .and flies, then I feel the presence of the Almighty . </p>
              </div>
            </div>

        </div>

    </div>
    
    <StartedSubSec/>

  </section>
</template>

<script>
import StartedSubSec from "@/components/StartedSubSec.vue";
export default {
name : "AboutUs",
components: {StartedSubSec
}
}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";
.box_text {
    .line_titles {
        @include sm_green_line;
        margin-left: 0;
    }
    span {
        font-size: $title_sec_size;
    }
    h2 {
        font-size: 65px;
        font-weight: bold;
        margin-top: 20px;
    }
    p {
        color: $title_grey_txt;
        font-size: 19px
    }

}


</style>