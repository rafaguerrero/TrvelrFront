<template>
  <div>
    <div id="header">
      <logo/>
    </div>
    <div id="content">
      <nuxt/>
    </div>
  </div>
</template>

<script>
  import Logo from '~/components/Logo.vue'

  export default {
    components: {
      Logo
    }
  }
</script>

<style>
  body {
    margin : 0;
    background-color: ivory;
  }

  #header {
    height: 45px;
    background-color: wheat;
    border-bottom: 1px solid black;
  }

  #content {
    width: 70%;
    margin: auto;
    padding-top: 15px;
  }
</style>

