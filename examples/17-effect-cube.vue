<style scoped>
  .swiper-container {
    width: 300px;
    height: 300px;
    position: absolute;
    left: 50%;
    top: 50%;
    margin-left: -150px;
    margin-top: -150px;
  }
  .swiper-slide {
    background-position: center;
    background-size: cover;
  }
</style>

<template>
  <div style="position: relative;overflow: hidden;height: 300px;">
    <div class="btn-group btn-vue-example">
      <button class="btn btn-default btn-xs btn-title">effect-cube</button>
      <button class="btn btn-default btn-xs btn-title">3D方块效果</button>
      <a href="https://github.com/surmon-china/vue-awesome-swiper/blob/master/examples/17-effect-cube.vue" target="_blank" class="btn btn-primary btn-xs">&lt; &gt;</a>
    </div>
    <swiper :options="swiperOption">
      <swiper-slide>Slide 1</swiper-slide>
      <swiper-slide>Slide 2</swiper-slide>
      <swiper-slide>Slide 3</swiper-slide>
      <swiper-slide>Slide 4</swiper-slide>
      <swiper-slide>Slide 5</swiper-slide>
      <swiper-slide>Slide 6</swiper-slide>
      <swiper-slide>Slide 7</swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        swiperOption: {
          pagination: '.swiper-pagination',
          effect: 'cube',
          grabCursor: true,
          cube: {
            shadow: true,
            slideShadows: true,
            shadowOffset: 20,
            shadowScale: 0.94
          }
        }
      }
    }
  }
</script>
