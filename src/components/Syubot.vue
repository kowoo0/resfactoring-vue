<template>
<div>
  <div class="syubot-header">
    <h2>너와 나의 친구, 삼육봇</h2>
  </div>
  <div class="mobile-frame">
    <div class="out-frame">
      <div class="in-frame">
        <img src="../assets/activity/syubot.png" width="100%" height="100%" />
      </div>
    </div>
  </div>
  <div class="syubot-intro">
    <h4>학교의 다양한 정보를 빠르게 얻을 수 있는 챗봇</h4>
    <h5>MVP 챌린지로 시작한 프로젝트가 현재 이용자 수는 무려 800명 가까이!!!</h5>
    <h5>아래 링크를 통해 개발 이야기를 더 살펴보세요</h5>
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

  background-color: gold;
}
.syubot-intro {
  width: 50%;

  float: right;
}
.syubot-intro > h4 {
  margin-top: 30px;
  margin-bottom: 30px;
}
.syubot-intro > h5 {
  margin-top: 20px;
}
@media (max-width: 768px) { 
  .syubot-header, .syubot-intro, .mobile-frame { float: none; }
  .syubot-header, .syubot-intro { width: 100%; }
  .mobile-frame { width: 80%; height: 100vmin; margin: 0 auto; }
}
</style>