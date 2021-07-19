<template>
  <section>
      <div class="box">
          <div class="row">

          <div class="left_side col">
              <img src="@/assets/images/business-people-working-together-on-project-and-5FHSKBL.jpg" alt="Consulting People">
          </div>
          <div class="right_side col px-5 d-flex align-items-center">
              <div class="box_text w-75">
                <div class="line_titles "></div>
                <span>ABOUT US</span>
                <h2>WE MAKE YOUR STRATEGY WORK</h2>
              </div>
              

          </div>

          </div>

      </div>
  </section>
</template>

<script>
export default {
name : "AboutUs"
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

}


</style>