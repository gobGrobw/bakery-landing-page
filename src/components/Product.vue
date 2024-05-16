<script setup>
import ProductTemplate from './ProductTemplate.vue';
</script>

<template>
	<!-- Product of Bakeries, Pastries & Brownies -->
	<ProductTemplate bgColor="#ececec" id="product-section">
		<template #title>
			<h1>Our Product</h1>
			<h3>
				Lorem ipsum dolor, sit amet consectetur adipisicing elit. Accusantium id totam quae,
				autem voluptatem eius, ipsam praesentium doloremque aliquid fugit commodi, iure
				quaerat dolores sed!
			</h3>
		</template>

		<template #product>
			<div class="card">
				<div id="container">
					<img class="yellow-border" src="../../images/cake.jpg" alt="Cakes" />
				</div>
				<p>Cakes</p>
			</div>

			<div class="card">
				<div id="container">
					<img class="yellow-border" src="../../images/pastry.jpg" alt="Pastries" />
				</div>
				<p>Pastries</p>
			</div>

			<div class="card">
				<div id="container">
					<img class="yellow-border" src="../../images/brownies.jpg" alt="Brownies" />
				</div>
				<p>Brownies</p>
			</div>
		</template>
	</ProductTemplate>

	<ProductTemplate bgColor="rgb(227, 188, 132)" id="snack-section">
		<template #title>
			<h1>Biteable Snacks</h1>
			<h3>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam harum amet dolores
				maxime enim suscipit a veritatis natus maiores, quod voluptatum hic tempore atque.
				Ab!
			</h3>
		</template>

		<template #product>
			<div class="card">
				<div id="container">
					<img class="white-border" src="../../images/macarons.jpg" alt="Cakes" />
				</div>
				<p>Macarons</p>
			</div>

			<div class="card">
				<div id="container">
					<img class="white-border" src="../../images/cupcakes.jpg" alt="Pastries" />
				</div>
				<p>Cupcakes</p>
			</div>

			<div class="card">
				<div id="container">
					<img class="white-border" src="../../images/fruitpies.jpg" alt="Brownies" />
				</div>
				<p>Fruit Pies</p>
			</div>

			<div class="card">
				<div id="container">
					<img class="white-border" src="../../images/donuts.jpg" alt="Brownies" />
				</div>
				<p>Donuts</p>
			</div>
		</template>
	</ProductTemplate>
</template>

<style scoped>
h1 {
	font-size: 3.3rem;
	margin-bottom: 15px;
	font-family: 'Lora';
}

h3 {
	font-family: Arial, Helvetica, sans-serif;
	font-weight: lighter;
	overflow-wrap: break-word;
	width: 50%;
	font-size: 1.3rem;
}

.card {
	display: flex;
	flex-direction: column;
	gap: 10px;

	text-align: left;
}

.card p {
	font-size: 1.7rem;
	font-weight: 500;
	font-family: 'Lora';
}

#container {
	overflow: hidden;
}

img {
	object-fit: cover;
	width: 15vw;
	height: 20vw;
	transition: 200ms ease-in-out;
}

.yellow-border {
	border: 7px solid rgb(227, 188, 132);
}

.white-border {
	border: 7px solid #ececec;
}

img:hover {
	transform: scale(1.1);
}

@media (max-width: 1200px) {
	img {
		width: 20vw;
		height: 20vw;
	}
}

@media (max-width: 815px) {
	.card p {
		text-align: center;
	}

	h1 {
		margin-bottom: 0;
		margin-top: 20px;
	}

	h3 {
		font-size: 1.1rem;
		width: 90%;
	}

	img {
		width: 250px;
		height: 250px;
	}
}
</style>

