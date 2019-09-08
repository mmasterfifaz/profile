<template>
  <div class="hello">
    <h3>{{ data.prename + ' ' + data.firstname + ' ' + data.lastname }}</h3>
    <!-- <ui>
        <li>อายุ: {{ data.age }}</li>
        <li>เบอร์โทรศัพท์: {{ data.phoneNumber }}</li>
    </ui> -->
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    data: Object
  }
  // ,
  // data() {
  //   return {
  //     fullname : this.data.prename + ' ' + this.data.firstname + ' ' + this.data.lastname
  //   }
  // },
  // methods: {
  //   getFullname(){
  //     let name = null
  //     if(this.data){
  //       if(this.data.prename){
  //         name = this.data.prename
  //       }
  //       if(this.data.firstname){
  //         name = name + ' ' + this.data.firstname
  //       }
  //       if(this.data.lastname){
  //         name = name + ' ' + this.data.lastname
  //       }
  //     }
  //     this.fullname = name
  //   }
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
