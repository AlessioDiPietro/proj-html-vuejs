<template>
  <section id="BLOG">
        <div class="container-fluid">

            <div class="row d-flex justify-content-between">

                <div class="blog_title p-0 col-7">
                    <div class="line_titles"></div>
                    <span>BLOG</span>
                    <h2>THE RECENT NEWS YOU MUST READ IT</h2>
                </div>

                <div class="btn_title p-0 col d-flex justify-content-end align-items-end">
                    <button class="btn_view">VIEW ALL</button>
                </div>
                


            </div>

            <div class="row mt-5 d-flex justify-content-between">
                <aside class="left">
                    <div class="text_content w-75 bg-light">
                        <label for="date">july, 4  2019</label>
                        <label for="host">by Paul</label>
                        <h3 class="my-4">Canadian Consulting Firm acquired by UK Giant </h3>
                        <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...</p>
                        
                    </div>
                </aside>

                <aside class="right">
                    <div class="text_content w-75 bg-light">
                        <label for="date">july, 4  2019</label>
                        <label for="host">by Paul</label>
                        <h3 class="my-4">Canadian Consulting Firm acquired by UK Giant </h3>
                        <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...</p>
                    </div>
                </aside>
            </div>

        </div>


  </section>
</template>

<script>
export default {
    name: "Blog"
}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";

section {
    @include form_section_90;
    padding-bottom: $margin_sec_top;
    .blog_title {
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
    .btn_view {
        @include btn_maringreen;
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
                    background-color: $int_red_bg;
                }
            }
        }
    }
    aside {
        width: calc(100% / 2 - 20px);
        height: 590px;
        color:black;
        position:relative;
        .text_content{
            position: absolute;
            right: -1px;
            bottom: 0;
            padding: 50px 90px;
            transform: translate(0 , 25%);
            label {
            color: $int_red_bg;
            margin-left: 20px;
            font-size: $title_sec_size;
            }
            h3{
            font-size: $title_sec_size_max;
            font-weight: bolder;
            }
            p {
            color: $parag_grey_txt;
            font-size: 19px
            }
        }
        
    }
    .left {
        background-image: url("../assets/images/startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg");
        background-size: cover;
        background-size: 100%;
        transition: all 1.5s;
        &:hover{
            background-size: 130%;
        }
        
    }
    .right {
        background-image: url("../assets/images/business-people-working-together-on-project-and-5FHSKBL-1390.jpg");
        background-position-y: center;
        background-size: 100%;
        transition: all 1.5s;
        &:hover{
            background-size: 130%;
        }
    }
}

</style>