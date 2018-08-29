<template>
  <div class='latest-trips'>
    <h2 class='latest-trips__title'>{{ title }}</h2>
    
    <template v-for="(post, index) in posts" >
      <trip-excerpt :key="index" 
                    :title="post.title"
                    :content="post.content"/>
    </template>
  </div>
</template>

<script>
  import TripExcerpt from '~/components/trips/TripExcerpt.vue'

  export default {
      components: {
        TripExcerpt
      },
      data() {
          return { 
            title: 'Latest Trips', 
            posts : [{
              title: "Trip 1",
              content: "This is the body of the trip 1"
            },{
              title: "Trip 2",
              content: "This is also an trip but the number 2"
            },{
              title: "Trip 3",
              content: "This trip is the third one"
            }]
          }
      }
  };
</script>

<style>
  .latest-trips__title {
    margin: 0;
    margin-bottom: 10px;
  }
</style>

