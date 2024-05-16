<template>
	<div class="body" id="about-us-section">
		<h1>About Us</h1>
		<div id="container">
			<h3>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum dolor sed veritatis
				accusamus sapiente? Blanditiis minus commodi nostrum officiis quis recusandae soluta
				maiores dolorum labore cumque aperiam ut hic, repellendus ullam atque animi
				praesentium, mollitia consequuntur! Perspiciatis, reprehenderit sint. Fugiat vitae
				sit mollitia magnam dolorem aperiam obcaecati dignissimos autem qui.
			</h3>
			<img
				src="https://images.unsplash.com/photo-1583338917451-face2751d8d5?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
				alt="Doe's Delight"
			/>
			<h3>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem, dignissimos
				quae? Quam maiores dolorum necessitatibus unde quasi sint obcaecati autem, labore
				voluptatibus voluptatum sed odio doloribus ut rem minima suscipit.
			</h3>
		</div>
	</div>
</template>

<style scoped>
.body {
	height: 60vh;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	background-color: #ececec;
}

.body h1 {
	padding: 25px;
	font-size: 3.3rem;
}

#container {
	display: flex;
	justify-content: center;
}

#container h3 {
	width: 20%;
	font-weight: lighter;
	font-family: Arial, Helvetica, sans-serif;
	padding: 20px;
	font-size: 1.2rem;
}

img {
	object-fit: cover;
	height: 30vh;
	width: 30vh;
	border: 10px solid rgb(227, 188, 132);
}

@media (max-width: 1250px) {
	.body {
		height: auto;
	}

	#container {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	#container h3 {
		width: 100%;
	}
}
</style>

