<template>
  <div id="app">
    <nav>
      <router-link to="/">Home</router-link>
    </nav>
    <transition name="view" enter-active-class="animated slideInRight">
      <router-view></router-view>
    </transition>
  </div>
</template>

<script>
import Skills from './components/Skills.vue'

export default {
  name: 'app',
  components: {
    Skills
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Montserrat');
  @import url('https://cdn.jsdelivr.net/npm/animate.css@3.5.2/animate.min.css');

  body { background: #eee; font-family: 'Montserrat', sans-serif; display: grid; grid-template-rows: auto; justify-items: center; align-items: center; padding-top: 50px; }
  body, html { margin: 0; height: 100%; }
  #app { width: 50%; }
  nav { padding: 20px 20px 20px 0; }
  nav a { padding: 10px; text-decoration: none; background: #fff; border-radius: 3px; color: rgb(0, 110, 255); font-weight: bold; margin-right: 15px; }
</style>
