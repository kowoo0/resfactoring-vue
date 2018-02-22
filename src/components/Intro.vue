<template>
<header id="intro">
  <div class="intro-cover-dark"></div>
  <div class="intro-body">
    <div class="container-fluid">
      <h1 class="intro-text">RESFACTORING</h1>
      <span class="static-text">We always wonder </span>
      <Typer/>
      <ApplyButton/>
    </div>
  </div>
</header>
</template>

<script>
import ApplyButton from './ApplyButton'
import Typer from './Typer'

export default {
  name: 'Intro',
  components: { Typer, ApplyButton },
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
  position: relative;

  display: table;
  width: 100%;
  height: 100vh;
  
  background: url(../assets/intro/introback.jpg);
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;

  text-align: center;
}
.intro-cover-dark {
  z-index: 1;
  position: absolute;
  left: 0px; top: 0px;
  width: 100%; height: 100vh;
  background: dimgray;
  opacity: 0.4;
}
.intro-body {
  position: relative;
  z-index: 3;
  display: table-cell;
  vertical-align: middle;
}
.intro-text {
  font-weight: 800;

  color: #fff;
  transition: 0.3s linear;
}
.intro-ads {
  margin-top: 120px;
}
.static-text {
  font-weight: 600;
  color: aquamarine;
}
@media (min-width: 0px) {
  .static-text { font-size: 1.2rem; }
}

/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) { 
  .static-text { font-size: 1.5rem; }
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) { 
  .static-text { font-size: 1.8rem; }
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) {
  .static-text { font-size: 2.1rem; }
}

/* Extra large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) { 
  .static-text { font-size: 2.4rem; }
}
</style>
