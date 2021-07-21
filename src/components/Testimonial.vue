<template>
  <section id="SERVICE">
      <div class="container-fluid">

        <div class="row">

            <div class="testimonial_title text-end">
                <div class="line_titles"></div>
                <span>Testimonial</span>
                <h2>WHAT'S THE CUSTOMER SAY ABOUT OUR WORK</h2>
            </div>

        </div>
        <div class="row box_content">
            <div class="box first">
                <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .</p>
                <h3>Vera Dunkan</h3>
                <div>Amazon Inc.</div>
            </div>
            <div class="box second">
                <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .</p>
                <h3>Vera Dunkan</h3>
                <div>Amazon Inc.</div>
            </div>
            <div class="box third">
                <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .</p>
                <h3>Vera Dunkan</h3>
                <div>Amazon Inc.</div>
                
            </div>
        </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "Testimonial",
}

</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";
section {
    @include form_section_right;
    margin-top: $margin_sec_top;
    .testimonial_title{
        width: 95%;
        .line_titles{
            @include sm_green_line;
        }
        span {
            font-size: $title_sec_size;
        }
        h2 {
            @include title_sec_name;
        }

    }
    .box_content{
        background-color: $white_bg;
        color: $dark_blue_txt;
        
        .box{
            display: inline-block;
            width: calc(100% / 3.6);
            font-size: 18px;
            padding: 45px 70px;
           
            h3{
                font-size: 33px;
                font-weight: bolder;
                margin-top: 30px;
            }
            
        }
        .first{
            background-image: none;
            transition:all 2s linear;
            &:hover{
                background-image: url("../assets/images/oliver-ragfelt-488196-2.jpg");
                h3{
                    color:$white_txt;
                }
                p {
                    color:$title_grey_txt;
                }
            }
        }
        .second{
            background-image: none;
            transition:all 1s linear;
            &:hover{
                background-image: url("../assets/images/oliver-ragfelt-488196-unsplash.jpg");
                h3{
                    color:$white_txt;
                }
                p {
                    color:$title_grey_txt;
                }
            }
        }
        .third{
            background-image: none;
            transition:all 1s linear;
            &:hover{
                background-image: url("../assets/images/12679.jpg");
                h3{
                    color:$white_txt;
                }
                p {
                    color:$title_grey_txt;
                }
            }
        }
    }

}
</style>