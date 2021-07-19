<template>
  <section class="d-flex justify-content-end">
      <div class="box">
          <span>OUR CONSULTANTS CAN HELP YOU</span>
          <div class="green_line"></div>
          <ul class="m-5">
              <li v-for="(items,index) in consultingData" :key="index">

                <i :class="items.icon" class="rounded-circle"></i>

                <span>{{items.title}}
                   <p>{{items.parag}}</p> 
                </span>

                  
              </li>
          </ul>
      </div>

  </section>
</template>

<script>
export default {
    name: "Consults",
    data(){
        return {
            consultingData: [
                {
                    title: "STATICAL CONSULTING",
                    parag: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
                    icon: "fas fa-chart-line"
                },
                {
                    title: "DIGITAL CONSULTING",
                    parag: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
                    icon: "fas fa-bullhorn"
                },
                {
                    title: "BANKING CONSULTING",
                    parag: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
                    icon: "fas fa-wallet"
                },
                {
                    title: "ENTERPRISE CONSULTING",
                    parag: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
                    icon: "fas fa-crosshairs"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";
    .box {
        width: 90%;
        height: 900px;
        padding-top: 120px;
        padding-left: 135px;
        background-color: $white_bg;
        color: black;
        font-weight: 600;
        span {
            font-size: 40px;
        }
        .green_line {
             display: inline-block;
            height: 3px;
            width: 54%;
            margin-left: 55px;
            background-color: $int_maringreen_bg;
            vertical-align: text-top;
        }
        li {
            list-style: none;
            width: 33%;
            display: inline-block;
            margin-right: 220px;
            margin-top: 90px;
            
            i {
                font-size: 45px;
                padding: 20px;
                background-color: $int_red_bg;
                color: white;
                margin-left: -110px;
                margin-right: 20px;
            }
            p {
                font-size: 16px;
                color: $parag_grey_txt;

            }
        }
    }

</style>