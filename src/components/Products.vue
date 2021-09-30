<template>
	<section>
		<!-- TODO: Pasquale -->
		<h2>Lista Prodotti</h2>
		<div class="products">
			<div class="product">
				<img class="product__image" src="https://www.lamolisana.it/wp-content/uploads/2021/04/1-spaghetto-quadrato.jpg" alt="">
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
				border: 1px solid black;

				.product__name{
					text-align: center;
				}

				.product__image{
					width: 100%;
				}
			}
		}
	}
</style>