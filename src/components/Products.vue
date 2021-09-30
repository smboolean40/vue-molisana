<template>
	<section>
		<!-- TODO: Pasquale -->
		<h2>Lista Prodotti</h2>
		<div class="products">
			<div class="product">
				<img src="https://picsum.photos/200/300" alt="">
				<div class="product__name">
					Nome Pasta
				</div>

			</div>

		</div>
	</section>
</template>

<script>
export default {
	name: "Products"
}
</script>

<style lang="scss" scoped>
	section {
		background-image: url("../assets/images/bg-prods.jpg");

		h2{
			text-align: center;
		}

		.products{
			display: flex;
			flex-wrap: wrap;
			width: 80%;
			margin: 0 auto;

			.product{
				width: 25%;
			}
		}
	}
</style>