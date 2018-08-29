<template>
  <section>
    <google-map/>
    
    <hr class='splitter'>

    <latest-trips/>
  </section>
</template>

<script>
  import GoogleMap from '~/components/GoogleMap.vue'
  import LatestTrips from '~/components/trips/LatestTrips.vue'

  export default {
    components: {
      GoogleMap,
      LatestTrips
    }
  }
</script>

<style>
  .splitter {
      margin: 25px 0;
  } 
</style>
