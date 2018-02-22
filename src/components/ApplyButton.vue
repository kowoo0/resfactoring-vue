<template>
<div>
  <div class="apply-btn-wrapper">
    <div class="apply-btn">
      <img class="apply-img" src="../assets/apply/google-form.png" width="20" height="20" alt="google-form" />
      <span class="apply-txt">APPLY</span>
    </div>
    <div class="apply-btn">
      <img class="apply-img" src="../assets/apply/github.svg" width="20" height="20" />
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
  margin-top: 80px;
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
  color: #343a40;
  letter-spacing: 1px;
  border-radius: 10px;

  box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease 0s;
  cursor: pointer;
  outline: none;
}
.apply-btn:hover {
  background-color: #2EE59D;
  box-shadow: 0px 15px 20px rgba(46, 229, 157, 0.4);
  color: #fff;
  transform: translateY(-7px);
}

.apply-btn:nth-of-type(2) { margin-left: 10px; }

.apply-img {
  float: left;
}

@media (max-width: 768px) {
  .apply-btn-wrapper { margin-top: 0px; }
  .apply-btn:nth-of-type(1) {
    margin-top: 20px;
  }
  .apply-btn:nth-of-type(2) {
    margin-top: 20px;
    margin-left: 0px;
  }
}
</style>