<template>
  <h1 id='trv-title'>{{ title }}</h1>
</template>

<script>
  export default {
      data() {
          return { title: 'Trvelr' }
      },
      methods: {
        onButtonClick() {
          console.log('------------------------');
          console.log("Clicking")
          console.log('------------------------');
        }
      }
  };
</script>

<style>
  #trv-title {
    color: black;
    margin : 0;
    padding : 0;
  }
</style>

