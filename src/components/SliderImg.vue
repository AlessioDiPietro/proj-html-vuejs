<template>
  <section>
      <div class="container-fluid">
          <div class="slide-box d-flex justify-content-around">

          <!-- <img :src=" require('@/assets/images/'+ image)" v-for="(image,counter) in sliderImgTake" :key="counter" :alt="image" class="col-4 mx-3">
          <span>{{counterSlide}}</span> -->
        

        <img :src=" require('@/assets/images/'+ sliderImgTake[counter1])" alt="" class="col-4 mx-3">
        <img :src=" require('@/assets/images/'+ sliderImgTake[counter2])" alt="" class="col-4 mx-3">
        <img :src=" require('@/assets/images/'+ sliderImgTake[counter3])" alt="" class="col-4 mx-3">

          </div>
        <button @click="nextSlide()">clicca</button> 
        <button @click="prevSlide()">clicca</button> 
          
          
          
          
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
            timer: null,
            counter1: 0,
            counter2: 1,
            counter3: 2
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
    }

}
</script>

<style lang="scss">

</style>