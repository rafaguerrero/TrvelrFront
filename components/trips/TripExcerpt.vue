<template>
  <div class='trip-excerpt'>
    <h3 class='trip-excerpt__title'>{{ title }}</h3>
    <p class='trip-excerpt__content'>{{ content }}</p>
  </div>
</template>

<script>
  export default {
		props: {
			title: {
				type: String,
				required: true
			},
			content: {
				type: String,
				required: true
			}
		}
	};
</script>

<style>
	.trip-excerpt {
		background-color: aliceblue;
		border: 1px solid black;
		margin-bottom: 15px;
		padding: 10px;
	}

	.trip-excerpt__title {
		margin: 0;
		margin-bottom: 10px;
	}

	.trip-excerpt__content {
		margin: 0;
	}
</style>