<template>
  <section>
      <div class="container-fluid position-relative w-100">
          <div class="btn_group position-absolute">
            <button @click="prevSlide()"><i class="fas fa-arrow-left"></i></button> 
            <button @click="nextSlide()"><i class="fas fa-arrow-right"></i></button> 
          </div>

            <div class="slide-box d-flex justify-content-around">



                <div class="img_box position-relative col-4 mx-3">
                    <img :src=" require('@/assets/images/'+ sliderImgTake[counter1])" alt="img demo" class="w-100">
                    <div class="add_comp position-absolute bottom-0 position-absolute w-100 d-flex justify-content-between align-items-center">
                        <div class="text_des">
                            <h4>Purinky Products</h4>
                            <h6>uncategorized</h6>
                        </div>
                        <div class="icon"><i class="fas fa-plus"></i></div>
                        

                    </div>
                </div>
                <div class="img_box position-relative col-4 mx-3">
                    <img :src=" require('@/assets/images/'+ sliderImgTake[counter2])" alt="img demo" class="w-100">
                    <div class="add_comp position-absolute bottom-0 w-100 d-flex justify-content-between align-items-center">
                        <div class="text_des">
                            <h4>Purinky Products</h4>
                            <h6>uncategorized</h6>
                        </div>
                        <div class="icon"><i class="fas fa-plus"></i></div>
                        

                    </div>
                </div>
                <div class="img_box position-relative col-4 mx-3">
                    <img :src=" require('@/assets/images/'+ sliderImgTake[counter3])" alt="img demo" class="w-100">
                    <div class="add_comp position-absolute bottom-0 w-100 d-flex justify-content-between align-items-center">
                        <div class="text_des">
                            <h4>Purinky Products</h4>
                            <h6>uncategorized</h6>
                        </div>
                        <div class="icon"><i class="fas fa-plus"></i>
                        </div>
                        

                    </div>
                </div>
                
                
                
            </div>
          
        </div>
  </section>
</template>

<script>
export default {
    name: "SlideImg",
    props:["sliderImgTake"],
    data(){
        return{
            counterSlide: this.sliderImgTake.length,
            counter1: 0,
            counter2: 1,
            counter3: 2,
            timer: ""
        }
    },
    methods:{
        nextSlide(){
            this.counter1 == this.counterSlide -1 ? this.counter1 = 0 : this.counter1++;
            this.counter2 == this.counterSlide -1 ? this.counter2 = 0 : this.counter2++;
            this.counter3 == this.counterSlide -1 ? this.counter3 = 0 : this.counter3++;
        },
        prevSlide(){
            this.counter1 == 0 ? this.counter1 = this.counterSlide -1 : this.counter1--;
            this.counter2 == 0 ? this.counter2 = this.counterSlide -1 : this.counter2--;
            this.counter3 == 0 ? this.counter3 = this.counterSlide -1 : this.counter3--;
        }
    },
    mounted() {
        this.timer= setInterval(this.nextSlide, 3000);
    }

}
</script>

<style lang="scss" scoped>
@import "@/assets/ColorPhloxVar.scss";
section {
    margin-top: 100px !important;
    width: 98% !important;
    .btn_group {
        top: -160px;
        right: 0;
        button{
            padding: 10px 15px;
            margin-left: 20px;
            border: none;
            background-color: rgba(110, 109, 110, 0.486);
        }
    }
    .slide-box{
        .img_box{
            background-color: $opa_red_bg;
            opacity: 1;
            .add_comp{
                display: none !important;
                padding: 15px;

                h4{
                    color:$white_txt;
                    font-weight: bolder;
                    font-size: 22px;
                }
                h6{
                    color: $title_grey_txt;
                    font-size: 18px;
                }
                        
                .icon {
                    font-size: 30px;
                    padding: 20px 30px;
                    margin-left: 10px;
                    background-color: $blue_bg;
                }
            }
            &:hover{
                img{
                    opacity: 0.2;
                }
                .add_comp{
                    display: flex !important;
                }
            }
        }
    }
}

    

        



</style>