<template>
<section id="activity">
  <div class="activity-body">
    <div class="container">
      <button type="button" class="btn btn-link">
        <router-link v-bind:to="{name:'syubot'}">삼육봇</router-link>
      </button>
      <button type="button" class="btn btn-link">
        <router-link v-bind:to="{name:'syubamboo'}">울창한대나무숲</router-link>
      </button>
      <button type="button" class="btn btn-link">
        <router-link v-bind:to="{name:'seminar'}">그외 활동들</router-link>
      </button>
    </div>
    <div class="container">
      <div class="activity-content">
        <router-view></router-view>
      </div>
    </div>
  </div>
</section>
</template>

<script>
import Syubot from './Syubot'
import Syubamboo from './Syubamboo'
import Seminar from './Seminar'
import VueRouter from 'vue-router';

const router = new VueRouter({
  mode : 'history',
  routes : [
    { path: '/', component: Syubot },
    { path: '/syubot', name: 'syubot', component: Syubot },
    { path: '/syubamboo', name: 'syubamboo', component: Syubamboo },
    { path: '/seminar', name: 'seminar', component: Seminar }
  ]
})

export default {
  name: 'Activity',
  router,
  data () {
    return {
      tmp: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#activity {
  width: 100%;
  height: 100vh;
  padding-top: 150px;
}
.activity-content {
  padding: 10px;
  overflow: hidden;
}
</style>
