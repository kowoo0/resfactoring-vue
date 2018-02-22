<template>
  <div id="app" v-cloak>
    <Nav/>
    <Intro/>
    <About/>
    <Programme/>
    <Activity/>
    <Apply/>
    <Footer/>
  </div>
</template>

<script>
import Nav from './components/Nav'
import Intro from './components/Intro'
import About from './components/About'
import Programme from './components/Programme'
import Activity from './components/Activity'
import Apply from './components/Apply'
import Footer  from './components/Footer'

export default {
  name: 'App',
  components: {
    Nav, Intro, About, Programme, Activity, Apply, Footer
  }
}
</script>

<style>
/* init */
* { margin: 0; padding: 0; box-sizing: border-box; }
html, body { width: 100%; height: 100%; }
body { position: relative; background: #F9F9F9; }
a { text-decoration: none; cursor: pointer; }
h1 { font-weight: 800; }
h2 { font-weight: 500; }

#app {
  font-family: 'Roboto', 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

@media (min-width: 0px) {
  h1 { font-size: 2.5rem; }
  h2 { font-size: 1.6rem;}
  h3 { font-size: 1.2rem; }
  h4 { font-size: 1rem; }
  h5 { font-size: 0.95rem; }
  h6 { font-size: 0.9rem; }
  p { font-size: 0.9rem; }
}

/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) { 
  h1 { font-size: 3.5rem; }
  h2 { font-size: 2.1rem;}
  h3 { font-size: 1.5rem; }
  h4 { font-size: 1.1rem; }
  h5 { font-size: 1.0rem; }
  h6 { font-size: 0.93rem; }
  p { font-size: 0.93rem; }
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) { 
  h1 { font-size: 4.5rem; }
  h2 { font-size: 2.4rem;}
  h3 { font-size: 1.8rem; }
  h4 { font-size: 1.2rem; }
  h5 { font-size: 1.1rem; }
  h6 { font-size: 1.03rem; }
  p { font-size: 1.03rem; }
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) {
  h1 { font-size: 5.5rem; }
  h2 { font-size: 2.8rem;}
  h3 { font-size: 2.1rem; }
  h4 { font-size: 1.3rem; }
  h5 { font-size: 1.2rem; }
  h6 { font-size: 1.1rem; }
  p { font-size: 1.1rem; }
}

/* Extra large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) { 
  h1 { font-size: 6.5rem; }
  h2 { font-size: 3.0rem;}
  h3 { font-size: 2.4rem; }
  h4 { font-size: 1.4rem; }
  h5 { font-size: 1.3rem; }
  h6 { font-size: 1.15rem; }
  p { font-size: 1.15rem; }
}

[v-cloak] { display: none; }
</style>
