<template>
<vue-typer
  :text='["Flow","Architecture","Optimizing","Latest Trend","Open Source"]'
  :repeat='Infinity'
  :shuffle='false'
  initial-action='typing'
  :pre-type-delay='70'
  :type-delay='70'
  :pre-erase-delay='2000'
  :erase-delay='86'
  erase-style='backspace'
  :erase-on-complete='false'
  caret-animation='phase'
></vue-typer>
</template>

<script>
import { VueTyper } from 'vue-typer'

export default {
  name: 'Typer',
  components: { VueTyper }
}
</script>

<style scoped>
.vue-typer {
  font-weight: 600;
  opacity: 0.8;
}

@media (min-width: 0px) {
  .vue-typer { font-size: 1.2rem; }
}

/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) { 
  .vue-typer { font-size: 1.5rem; }
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) { 
  .vue-typer { font-size: 1.8rem; }
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) {
  .vue-typer { font-size: 2.1rem; }
}

/* Extra large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) { 
  .vue-typer { font-size: 2.4rem; }
}
</style>