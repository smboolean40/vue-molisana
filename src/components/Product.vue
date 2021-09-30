<template>
	<div class="product">
		<img class="product__image" :src="prod.src" :alt="prod.titolo">
		<div class="product__name">
			{{prod.titolo}}
		</div>
	</div>
</template>

<script>
export default {
	name: "Product",
	props: ['prod']
}
</script>

<style lang="scss" scoped>
	.product{
		width: 25%;
		border: 2px solid #dbe9ff;
		background-color: #fff;
		padding: 25px 0;

		.product__name{
			text-align: center;
			font-weight: 500;
			width: 60%;
			margin: 0 auto;
		}

		.product__image{
			width: 100%;
		}
	}
</style>