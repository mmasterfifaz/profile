<template>
  <div>
    <Main/>
    <!-- <div id="app">
      <Header />
      <img alt="Vue logo" src="./assets/logo.png">
      <HelloWorld msg="Welcome to Your Vue.js App"/>
    </div> -->
  </div>
</template>

<script>
import Vue from 'vue'
import VueMaterial from 'vue-material'
import 'vue-material/dist/vue-material.min.css'

// import HelloWorld from './components/HelloWorld.vue'
// import Header from './components/Header.vue'
import Main from './components/Main.vue'
import axios from 'axios'
import VueAxios from 'vue-axios'
 
Vue.use(VueAxios, axios)


Vue.use(VueMaterial)

export default {
  name: 'app',
  components: {
    Main
    // HelloWorld,
    // Header
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
