<template>
<div>
  <div class="apply-btn-wrapper">
    <div class="apply-btn">
      <img class="apply-img" src="../assets/apply/google-form.png" width="40" height="40" alt="google-form" />
      <span class="apply-txt">APPLY</span>
    </div>
    <div class="apply-btn">
      <img class="apply-img" src="../assets/apply/github.svg" width="40" height="40" />
      <span class="apply-txt">GITHUB</span>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'ApplyButton',
}
</script>

<style scoped>
.apply-btn-wrapper {
  padding: 5px 20px;  
}
.apply-btn {
  display: inline-block;

  padding: 10px;
  width: 200px;
  height: 60px;
  border: 1px solid #eaeaea;
  border-radius: 2px;
  background-color: #fff;
  line-height: 40px;
  font-size: 17px;
  font-weight: 600;
  letter-spacing: 1px;
}
.apply-img {
  float: left;
}
.apply-txt {
  color: #000;
  opacity: 0.8;
}

@media (max-width: 768px) {
  .apply-btn:nth-of-type(2) {
    margin-top: 10px;
  }
}
</style>