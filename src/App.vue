<script setup>
import Product from './components/Product.vue';
import Arrow from './components/icons/Arrow.vue';
import MenuHeader from './components/MenuHeader.vue';
import BackgroundSlider from './components/BackgroundSlider.vue';
</script>

<template>
	<!-- Background + Overlay -->
	<!-- <div class="background"> -->
	<BackgroundSlider>
		<MenuHeader />
		<div class="overlay center">
			<!-- Title -->
			<main class="center">
				<div id="title" class="center">
					<h1>Doe's Delight</h1>
					<div class="subtitle">
						<h3>Gourmet Bakery & Pastries</h3>
						<h2>A bite with a thousand flavours</h2>
					</div>
				</div>

				<button><a href="#product-section">Explore More</a></button>
				<Arrow />
			</main>
		</div>
	</BackgroundSlider>
	<!-- </div> -->
	<Product />
</template>

<style scoped>
a {
	color: white;
	text-decoration: none;
}

.overlay {
	background-color: rgba(0, 0, 0, 0.15);
	height: 100%;
}

.center {
	display: flex;
	justify-content: center;
	align-items: center;
}

/* Styling product button */
main {
	display: flex;
	flex-direction: column;
	gap: 20px;
}

main button {
	border: 0;
	border-radius: 5px;
	color: white;
	background: rgb(87, 60, 19);
	font-size: 1.7rem;
	font-weight: bold;
	padding: 10px 15px 10px 15px;
	cursor: pointer;
	transition: 100ms ease-in-out;
}

main button:hover {
	background-color: rgb(112, 77, 24);
}

/* Styling title */
#title {
	display: flex;
	flex-direction: column;
	color: white;
	line-height: 8vh;
	gap: 25px;
}

#title h1 {
	font-family: cursive;
	font-size: 8rem;
}

#title h2 {
	font-family: 'Times New Roman', Times, serif;
	font-size: 2.3rem;
}

#title h3 {
	font-family: 'Times New Roman', Times, serif;
	font-size: 1.8rem;
}

#title h1,
#title h2,
#title h3 {
	text-shadow: 1px 1px 2px black;
}

.subtitle {
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	line-height: 4vh;
}
</style>

