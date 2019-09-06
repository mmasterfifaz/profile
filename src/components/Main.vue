<template>
  <div class="page">
      <div class="hearder">
          <Header/>
          <!-- <HelloWorld/>           -->
          <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
      </div>
      <div class="body">
          <HelloWorld/>
      </div>
      <div class="footer">
        <Footer/>
      </div>
  </div>
</template>

<script>
import Header from './Header'
import HelloWorld from './HelloWorld'
import Footer from './Footer'

export default {
  name: 'Main',
  components: {
      Header,
      HelloWorld,
      Footer
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
