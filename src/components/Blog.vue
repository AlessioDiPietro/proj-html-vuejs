<template>
  <section>
        <div class="container-fluid">

            <div class="row d-flex justify-content-between">

                <div class="blog_title col-7">
                    <div class="line_titles"></div>
                    <span>BLOG</span>
                    <h2>THE RECENT NEWS YOU MUST READ IT</h2>
                </div>

                <div class="btn_title col d-flex justify-content-end align-items-end">
                    <button>VIEW ALL</button>
                </div>
                


            </div>

            <div class="row d-flex justify-content-between">
                <aside class="left col-5">
                    <div class="text_content">
                        <label for="date">july, 4  2019</label>
                        <label for="host">by Paul</label>
                        <h3>Canadian Consulting Firm acquired by UK Giant </h3>
                        <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...</p>
                        
                    </div>
                </aside>

                <aside class="right col-5">
                    <div class="text_content">
                        <label for="date">july, 4  2019</label>
                        <label for="host">by Paul</label>
                        <h3>Canadian Consulting Firm acquired by UK Giant </h3>
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
    .left {
        background-image: url(../assets/images/startup-business-people-and-strategy-board-PAJ3P9K-1390X1042.jpg);
    }
}

</style>