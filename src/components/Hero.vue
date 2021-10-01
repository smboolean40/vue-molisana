<template>
	<div class="hero" :style="`background-image: url(${bgImage})`">
		<h2>{{title}}</h2>
	</div>
</template>

<script>
export default {
	name: "Hero",
	props: [
		'bgImage',
		'title'
	]
}
</script>

<style scoped>
	.hero {
		height: 25rem;
		background-position: center;
		background-size: cover;
		position: relative;
	}

	h2 {
		position: absolute;
		bottom: 40px;
		left: 50%;
		transform: translateX(-50%);
	}
</style>