<template>
  <section>
      <div class="container-fluid position-relative w-100">
          <div class="btn_group position-absolute">
            <button @click="prevSlide()">prev</button> 
            <button @click="nextSlide()">next</button> 
          </div>

            <div class="slide-box d-flex justify-content-around">

                <img :src=" require('@/assets/images/'+ sliderImgTake[counter1])" alt="img demo" class="col-4 mx-3">
                <img :src=" require('@/assets/images/'+ sliderImgTake[counter2])" alt="img demo" class="col-4 mx-3">
                <img :src=" require('@/assets/images/'+ sliderImgTake[counter3])" alt="img demo" class="col-4 mx-3">

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
section {
    margin-top: 100px !important;
    width: 98% !important;
    .btn_group {
    top: -160px;
    right: 0

}
}


</style>