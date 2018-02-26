<template>
<footer>
<h3 class="footer-txt">#Resfactoring #리펙 #2기 #삼육대코딩파티</h3>
</footer>
</template>

<script>
export default {
  name: 'Footer',
  data () {
    return {
      tmp: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
footer {
  width: 100%;
  height: 80px;
  background: darkturquoise;
  opacity: 0.9;

  /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center; 
}
.footer-txt {
  margin: 0;
  color: whitesmoke;
  font-weight: bold;
  font-family: 'Nanum Pen Script', cursive;  
  text-align: center;
}
</style>
