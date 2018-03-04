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
  opacity: 0.9;
  background: #f9f9f9;

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

  -webkit-box-shadow: 0px -2px 2px 0px aquamarine;
  -moz-box-shadow: 0px -2px 2px 0px aquamarine;
  box-shadow: 0px -2px 2px 0px aquamarine;
}
.footer-txt {
  margin: 0;
  color: darkturquoise;
  font-weight: bold;
  font-family: 'Nanum Pen Script', cursive;  
  text-align: center;
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) {
  .footer-txt { font-size: 1.2rem; }
}
</style>
