<template>
  <div class="page">
      <div class="hearder">
          <Header/>
          <!-- <HelloWorld/>           -->
          <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
      </div>
      <div class="body">
          <HelloWorld :data="personal"/>
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

import axios from 'axios';

export default {
  name: 'Main',
  components: {
      Header,
      HelloWorld,
      Footer
  },
  data() {
    return {
      personal: null,
      address: null
    }
  },
  methods: {
    getPerson() {
      axios.get(`http://localhost:8081/userDetail`).then(res => {
        this.personal = res.data.result.personal
        this.address = res.data.result.address
      }).catch(e => { 
        console.log(e) 
      })
    }
  },
  mounted() {
    this.getPerson();
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
