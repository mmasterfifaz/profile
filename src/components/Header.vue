<template>
  <div class="header">
    <md-toolbar>
      <img class="logo" alt="Vue logo" src="../assets/logo.png" width="50" height="25">
      <h3 class="md-title" style="flex: 1">Home</h3>
      <md-button class="md-icon-button">
        <img class="logo" alt="Vue logo" src="../assets/user.png">
        <!-- <md-icon>more_vert</md-icon> -->
      </md-button>
    </md-toolbar>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
 .md-toolbar + .md-toolbar {
    margin-top: 16px;
  }
</style>
