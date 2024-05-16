<script setup>
import Arrow from './components/icons/Arrow.vue';
import MenuHeader from './components/MenuHeader.vue';
import BackgroundSlider from './components/BackgroundSlider.vue';
import Product from './components/Product.vue';
import AboutUs from './components/AboutUs.vue';
import Footer from './components/Footer.vue';
</script>

<template>
	<!-- Main Section -->
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

	<!-- Product Section -->
	<Product />
	<AboutUs />
	<Footer />
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
	z-index: 3;
}

main button {
	border: 0;
	border-radius: 5px;
	color: white;
	background: rgba(87, 60, 19, 0.7);
	font-size: 1.7rem;
	font-weight: bold;
	padding: 10px 15px 10px 15px;
	cursor: pointer;
	transition: 200ms ease-in-out;
}

main button:hover {
	background: rgb(87, 60, 19);
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

@media (max-width: 715px) {
	#title h1 {
		text-align: center;
		line-height: 100px;
	}

	#title h2,
	#title h3 {
		text-align: center;
	}
}
</style>

