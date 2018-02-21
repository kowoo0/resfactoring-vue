<template>
<div class="seminar">
<swiper :options="swiperOption" ref="mySwiper" class="swiper-box">
  <!-- slides -->
  <swiper-slide class="swiper-item"></swiper-slide>
  <swiper-slide class="swiper-item"></swiper-slide>
  <swiper-slide class="swiper-item"></swiper-slide>
  <swiper-slide class="swiper-item"></swiper-slide>
  <!-- Optional controls -->
  <div class="swiper-pagination"  slot="pagination"></div>
  <div class="swiper-button-prev" slot="button-prev"></div>
  <div class="swiper-button-next" slot="button-next"></div>
</swiper>
</div>
</template>

<script>
import 'swiper/dist/css/swiper.css'

import { swiper, swiperSlide } from 'vue-awesome-swiper'

export default {
  name: 'Seminar',
  components: { swiper, swiperSlide },
  data() {
    return {
      swiperOption: {
        slidesPerView: 1,
        spaceBetween: 30,
        mousewheel: true,
        pagination: {
          el: '.swiper-pagination',
          clickable: true
        },
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev',
        },
      }
    };
  },
}
</script>

<style scoped>
.seminar {
  margin-top: 70px;
  height: 50vmin;
}
.swiper-box {
    width: 100%;
    height: 100%;
    margin: 0 auto;
}
.swiper-item {
  height: 100%;
  text-align: center;
  font-size: 18px ;
  background: #fff;
}
</style>