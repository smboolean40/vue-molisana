<template>
	<footer class="container">
		<!-- TODO: Maria -->
		<div class="logo">
			<img src="@/assets/images/logo.png" alt="">
		</div>
		<div class="list">
			<h2>PASTIFICIO</h2>
			<ul v-for ="(link, index) in menu" :key="index">
				<li>{{link.nameLink}}</li>
			</ul>
		</div>
			<div class="list">
			<h2>PRODOTTI</h2>
			<ul v-for ="(link, index) in menu" :key="index">
				<li>{{link.nameLink}}</li>
			</ul>
		</div>
		
		
		
	</footer>
</template>

<script>
export default {
	name: "Footer",
	data(){
    return{
      menu:[
        {
          nameLink: "Il pastificio",
        },
		{
          nameLink: "Grano",
        },
		{
          nameLink: "Filiera",
        },
		{
          nameLink: "100 anni di pasta",
        },
		{
          nameLink: "Sartoria della pasta",
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
	// .container {
	// 	@import "../assets/style/variables";
	// 	max-width: $sizeContainer;
	// 	margin: 0 auto;
	// }
footer{
	display: flex;
	padding: 40px;
	background-image: url("../assets/images/footer.jpg");
	background-repeat: no-repeat;
	
}
.list{
	margin: 0 50px;
	ul{
		list-style: none;
	}
	li {
		font-size: 13px;
	}
	h2{
		@import '../assets/style/variables';
		margin-bottom: 15px;
		color: $mainColor;
	}
}

</style>