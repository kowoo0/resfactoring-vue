<template>
<div class="syubot">
  <div class="syubot-header" data-aos="fade-down" data-aos-duration="800">
    <h2>너와 나의 친구, 삼육봇</h2>
  </div>
  <div class="mobile-frame" data-aos="fade-right" data-aos-duration="800">
    <div class="out-frame">
      <div class="in-frame">
        <img src="../assets/activity/syubot.jpg" width="100%" height="100%" />
      </div>
    </div>
  </div>
  <div class="syubot-intro" data-aos="fade-left" data-aos-duration="800">
    <h4>학교의 다양한 정보를 빠르게 얻을 수 있는 챗봇</h4>
    <h5>MVP 챌린지로 시작한 프로젝트가 현재 이용자 수는 무려 800명 가까이!!!</h5>
    <h6>아래 링크를 통해 개발 이야기를 더 살펴보세요</h6>
    <a class="btn btn-primary btn-lg" href="#" role="button">Read more</a>
  </div>
</div>
</template>

<script>
export default {
  name: 'Syubot',
}
</script>

<style scoped>
.syubot-header {
  margin-top: 30px;
  margin-bottom: 20px;
  width: 50%; 

  color: gold;

  float: right;
}
.mobile-frame {
  width: 360px; height: 640px;
  float: left;
}
.mobile-frame .out-frame {
  padding: 10% 5%;
  width: 100%; height: 100%;

  border: 1px solid #e5e5e5;
  border-radius: 25px;

  -webkit-box-shadow: 0px 6px 12px 0px rgba(196,196,196,1);
  -moz-box-shadow: 0px 6px 12px 0px rgba(196,196,196,1);
  box-shadow: 0px 6px 12px 0px rgba(196,196,196,1);  
}
.mobile-frame .in-frame {
  width: 100%; height: 100%;
  border: 1px solid #e5e5e5;

  background-color: gold;
}
.syubot-intro {
  width: 50%;

  float: right;
}
.syubot-intro > h4 {
  margin-top: 30px;
  margin-bottom: 30px;

  color: #000;
  opacity: 0.8;
}
.syubot-intro > h5 {
  margin-top: 20px;

  color: #000;
  opacity: 0.7;
}
.syubot-intro > h6 {
  margin-top: 30px;
  margin-bottom: 30px;
  color: darkgrey;
}
.btn {
  background-color: gold;
  border-color: gold;
}



@media (min-width: 0px) and (max-width: 576px) {
  .syubot-header, .syubot-intro, .mobile-frame { float: none; }
  .syubot-header, .syubot-intro { width: 100%; }
  .mobile-frame {
    width: 80%; height: 120vmin; margin: 0 auto;
  }
}

/* Small devices (landscape phones, 576px and up) */
@media (min-width: 577px) and (max-width: 768px) { 
  .syubot-header, .syubot-intro, .mobile-frame { float: none; }
  .syubot-header, .syubot-intro { width: 100%; }
  .mobile-frame { width: 80%; height: 70vh; margin: 0 auto; }
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) and (max-width: 992px) { 
  .mobile-frame { width: 300px; height: 560px; }
}
</style>