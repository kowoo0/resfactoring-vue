<template>
<div>
  <h5 class="seminar-header">2기 활동사진이 추가될 공간입니다!</h5>
  <div class="seminar">
  <swiper :options="swiperOption" ref="mySwiper" class="swiper-box">
    <!-- slides -->
    <swiper-slide class="swiper-item">
      <img src="../assets/activity/git-seminar.jpg"
        width="100%" height="100%" alt="git" />
      <div class="dark-cover"></div>
      <div class="slide-desc">
        <h3>GIT 세미나</h3>
        <h5><a href="https://www.slideshare.net/JungHoonLee41/5-git-github" target="_blank">Slideshare로 더 살펴보기</a></h5>
      </div>
    </swiper-slide>
    <swiper-slide class="swiper-item">
      <img src="../assets/activity/aws-seminar.jpg"
        width="100%" height="100%" alt="aws" />
      <div class="dark-cover"></div>
      <div class="slide-desc">
        <h3>AWS 세미나</h3>
        <h5><a href="https://www.slideshare.net/JungHoonLee41/6-aws" target="_blank">Slideshare로 더 살펴보기</a></h5>
      </div>
    </swiper-slide>
    <swiper-slide class="swiper-item">
      <div class="dark-cover"></div>
      <div class="slide-desc">
        <h2>추가될 예정입니다</h2>
      </div>
    </swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
    <div class="swiper-button-prev" slot="button-prev"></div>
    <div class="swiper-button-next" slot="button-next"></div>
  </swiper>
  </div>
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
  height: 50vmin;

  -webkit-box-shadow: 0 8px 6px -6px black;
    -moz-box-shadow: 0 8px 6px -6px black;
        box-shadow: 0 8px 6px -6px black;
}
.seminar-header {
  margin-bottom: 12px;
}
.swiper-box {
    width: 100%;
    height: 100%;
    margin: 0 auto;
}
.swiper-item {
  position: relative;
  height: 100%;
  text-align: center;
  font-size: 18px ;
  background: #fff;
}
.dark-cover {
  position: absolute;
  left: 0px; top: 0px;
  width: 100%; height: 100%;
  background: #000;
  opacity: 0.5;
}
.slide-desc {
  position: absolute;
  left: 0px; top: 0px;
  width: 100%; height: 100%;
  padding: 10px;
  color: #fff;

  /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center; 
}
.slide-desc > h5 {
  margin-left: 20px;
}
.slide-desc > h5 > a {
  color: #fff;
}
</style>