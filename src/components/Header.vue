<template>
	<header>
		<div class="logo">
			<img :src="require('../assets/images/' + logo)" alt="Logo Molisana">
		</div>
		<nav>
			<ul>
				<li v-for="(link, index) in menu" :key="index">
					<a :href="link.url" :class="{ active : link.current }">{{link.text}}</a>
				</li>
			</ul>
		</nav>
	</header>
</template>

<script>
export default {
	name: "Header",
	data() {
		return {
			menu: [
                {
                    text: "Home",
                    url: "#",
                    current: false,
                },
                {
                    text: "Prodotti",
                    url: "#",
                    current: true,
                },
                {
                    text: "Chi Siamo",
                    url: "#",
                    current: false,
                },
                {
                    text: "Contatti",
                    url: "#",
                    current: false,
                },
            ],
			logo: "logo.png"
		}
	}
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables";

header {
	text-align: center;

	nav {

		margin: 1.5625rem 0;

		ul {
			display: flex;
			justify-content: center;
			list-style: none;
		}


		a {
			display: inline-block;
			text-decoration: none;
			padding: 1.25rem;
			color: $mainColor;
			font-size: 1.125rem;
			font-weight: 500;

			&.active {
				background-color: #DBE9FF;
			}
		}
	}
}

</style>