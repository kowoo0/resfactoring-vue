<template>
<div class="syubamboo">
  <div class="syubamboo-header">
    <h2>울창한 대나무숲</h2>
  </div>
  <div class="mobile-frame">
    <div class="out-frame">
      <div class="in-frame">
        <img src="../assets/activity/syubamboo.png" width="100%" height="100%" />
      </div>
    </div>
  </div>
  <div class="syubamboo-intro">
    <h4>삼육대학교의 다양한 커뮤니티사이트들의 글을 한눈에 볼 수 있는 웹 애플리케이션</h4>
    <h5>교내 프로젝트 경진대회에 출전해 우수상을 탔습니다!!</h5>
    <h6>아래 링크를 통해 개발 이야기를 더 살펴보세요</h6>
    <a class="btn btn-primary btn-lg" href="#" role="button">Read more</a>
  </div>
</div>
</template>

<script>
export default {
  name: 'Syubamboo',
}
</script>

<style scoped>
.syubamboo-header {
  margin-top: 30px;
  margin-bottom: 20px;
  width: 50%; 

  color: dodgerblue;

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

  background-color: dodgerblue;
}
.syubamboo-intro {
  width: 50%;

  float: right;
}
.syubamboo-intro > h4 {
  margin-top: 30px;
  margin-bottom: 30px;

  color: #000;
  opacity: 0.8;
}
.syubamboo-intro > h5 {
  margin-top: 20px;

  color: #000;
  opacity: 0.7;
}
.syubamboo-intro > h6 {
  margin-top: 30px;
  margin-bottom: 30px;
  color: darkgrey;
}

@media (min-width: 0px) and (max-width: 576px) {
  .syubamboo-header, .syubamboo-intro, .mobile-frame { float: none; }
  .syubamboo-header, .syubamboo-intro { width: 100%; }
  .mobile-frame {
    width: 80%; height: 120vmin; margin: 0 auto;
  }
}

/* Small devices (landscape phones, 576px and up) */
@media (min-width: 577px) and (max-width: 768px) { 
  .syubamboo-header, .syubamboo-intro, .mobile-frame { float: none; }
  .syubamboo-header, .syubamboo-intro { width: 100%; }
  .mobile-frame { width: 80%; height: 70vh; margin: 0 auto; }
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) and (max-width: 992px) { 
  .mobile-frame { width: 300px; height: 560px; }
}
</style>