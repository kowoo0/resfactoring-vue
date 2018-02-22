<template>
<section id="apply">
  <div class="apply-body">
    <div class="container">
      <div class="apply-txt">
        <h3>2기 모집기간 : 3월 5일 ~ 3월 14일</h3>
        <h1>지원하러가기</h1>
        <p>개발이 재밌고 함께 성장하는 것에 가치를 느끼시는 분, 자신의 소스를 오픈하는 '오픈소스' 개발에 관심있으신 분, 나는 개발자다! 부족하지만 열정이 넘치는 36학생 개발자의 많은 지원부탁드립니다!</p>
      </div>
    </div>
  </div>
</section>
</template>

<script>
export default {
  name: 'Apply',
  data () {
    return {
      tmp: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#apply {
  display: table;
  width: 100%;
  height: 100vh;
}
.apply-body {
  display: table-cell;
  vertical-align: middle;
}
.apply-txt {
  text-align: center;
}
</style>
