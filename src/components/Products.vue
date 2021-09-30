<template>
	<section>
		<!-- TODO: Pasquale -->
		<h2>Lista Prodotti</h2>
		<div class="products container">
			<div class="product">
				<img class="product__image" src="https://www.lamolisana.it/wp-content/uploads/2021/04/1-spaghetto-quadrato.jpg" alt="">
				<div class="product__name">
					N.4 Spaghetto Quadrato Bucato
				</div>

			</div>
			<div class="product">
				<img class="product__image" src="https://www.lamolisana.it/wp-content/uploads/2021/04/1-spaghetto-quadrato.jpg" alt="">
				<div class="product__name">
					N.4 Spaghetto Quadrato Bucato
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
@import "../assets/style/variables.scss";


	section {
		background-image: url("../assets/images/bg-prods.jpg");
		padding-top: 60px;
		color: $mainColor;

		h2{
			text-align: center;
			margin-bottom: 40px;
		}

		.products{
			display: flex;
			flex-wrap: wrap;

			.product{
				width: 25%;
				margin: 2px;
				background-color: #fff;
				padding: 25px 0;

				.product__name{
					text-align: center;
					font-weight: 500;
				}

				.product__image{
					width: 100%;
				}
			}
		}
	}
</style>