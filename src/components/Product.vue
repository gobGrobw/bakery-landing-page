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
					<img
						class="yellow-border"
						src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?q=80&w=1989&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
						alt="Cakes"
					/>
				</div>
				<p>Cakes</p>
			</div>

			<div class="card">
				<div id="container">
					<img
						class="yellow-border"
						src="https://images.unsplash.com/photo-1617026061250-62b474264442?q=80&w=2069&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
						alt="Pastries"
					/>
				</div>
				<p>Pastries</p>
			</div>

			<div class="card">
				<div id="container">
					<img
						class="yellow-border"
						src="https://images.unsplash.com/photo-1606313564573-104197cf8f91?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
						alt="Brownies"
					/>
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
					<img
						class="white-border"
						src="https://images.unsplash.com/photo-1596350351182-c2ce5b74a758?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
						alt="Cakes"
					/>
				</div>
				<p>Macarons</p>
			</div>

			<div class="card">
				<div id="container">
					<img
						class="white-border"
						src="https://images.unsplash.com/photo-1599785209707-a456fc1337bb?w=400&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8N3x8Y3VwY2FrZXN8ZW58MHx8MHx8fDA%3D"
						alt="Pastries"
					/>
				</div>
				<p>Cupcakes</p>
			</div>

			<div class="card">
				<div id="container">
					<img
						class="white-border"
						src="https://images.unsplash.com/photo-1495147466023-ac5c588e2e94?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
						alt="Brownies"
					/>
				</div>
				<p>Fruit Pies</p>
			</div>

			<div class="card">
				<div id="container">
					<img
						class="white-border"
						src="https://images.unsplash.com/photo-1551024601-bec78aea704b?w=400&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Mnx8ZG9udXRzfGVufDB8fDB8fHww"
						alt="Brownies"
					/>
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

