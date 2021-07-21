<template>
  <section id="PROJECT">
      <div class="container-fluid">

          <div class="row d-flex">

                <div class="project_title col-7">
                    <div class="line_titles"></div>
                    <span>PROJECT</span>
                    <h2>OUR EXPERT TRUSTED CONSULTANTS HELP CLIENTS</h2>
                </div>

            </div>

        </div> 
        <SliderImg :sliderImgTake="imgSlider"/> 
  </section>
</template>

<script>
import SliderImg from "@/components/SliderImg.vue"
export default {
name: "Project",
components: {
    SliderImg,
},
props:["imgSlider"]
}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";

section {
    @include form_section_90;
    .project_title {
        .line_titles{
            @include sm_green_line;
            margin-left: 0;
        }
        span {
            font-size: $title_sec_size;
        }
        h2 {
            @include title_sec_name;
        }

    }
}
</style>