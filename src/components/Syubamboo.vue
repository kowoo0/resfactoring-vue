<template>
<div>
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
    <h5>아래 링크를 통해 개발 이야기를 더 살펴보세요</h5>
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
  margin-bottom: 20px;
  width: 368px; height: 685px;

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

  background-color: lightskyblue;
}
.syubamboo-intro {
  width: 50%;

  float: right;
}
.syubamboo-intro > h4 {
  margin-top: 30px;
  margin-bottom: 30px;
}
.syubamboo-intro > h5 {
  margin-top: 20px;
}
@media (max-width: 768px) { 
  .syubamboo-header, .syubamboo-intro, .mobile-frame { float: none; }
  .syubamboo-header, .syubamboo-intro { width: 100%; }
  .mobile-frame { width: 80%; height: 100vmin; margin: 0 auto; }
}
</style>