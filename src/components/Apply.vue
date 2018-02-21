<template>
<section id="apply">
  <div class="apply-body">
    <div class="container-fluid">
      <div class="apply-txt">
        <h3>2기 모집기간 : 3월 2일 ~ 3월 14일</h3>
        <h1>지원하러가기</h1>
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
