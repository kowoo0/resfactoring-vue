<template>
<header id="intro">
  <div class="intro-body">
    <div class="container-fluid">
      <h1 class="intro-text">RESFACTORING</h1>
      <Test/>
      <ApplyButton/>
    </div>
  </div>
</header>
</template>

<script>
import Test from './Test.vue'
import ApplyButton from './ApplyButton'

export default {
  name: 'Intro',
  components: { Test, ApplyButton },
  data () {
    return {
      tmp: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#intro {
  display: table;
  width: 100%;
  height: 100vh;
  
  /* background: url(../assets/all4.svg);
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat; */

  text-align: center;
}
.intro-body {
  display: table-cell;
  vertical-align: middle;
}
.intro-text {
  font-weight: 800;

  transition: 0.3s linear;
}
.intro-ads {
  margin-top: 120px;
}
</style>
