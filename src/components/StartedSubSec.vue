<template>
  <section>
      <div class="container-fluid bg_green position-relative">
          <div class="row">
              <div class="d-flex justify-content-around align-items-center p-5">
                  <h3 class="w-25">WE HELP TO DELIVER THE BUSINESS CASE</h3>
                  <p class="w-25">When, while lovely valley teems with vapour around meand meridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown</p>
              </div>
            </div>
            <button class="position-absolute bottom-0 end-0 started_btn">GET STARTED</button>

      </div>
  </section>
</template>

<script>
export default {
    name: "StartedSubSec"

}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";
section{
    @include form_section_left;
}
.bg_green {
    background-color: $opa_maringreen_bg;
    padding: 50px 160px;
    color: $dark_blue_txt;
    h3 {
        font-size: 33px;
        font-weight: bolder;
    }
    p {
        font-size: 18px;
    }
    .started_btn{
        @include btn_red;
    }
}

</style>