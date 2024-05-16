<template>
	<div id="body">
		<ul>
			<li><a href="#product-section">Products</a></li>
			<li><a href="#snack-section">Snacks</a></li>
			<li><a href="#about-us-section">About Us</a></li>
		</ul>
	</div>
</template>

<style scoped>
#body {
	position: fixed;
	z-index: 10; /* Make sure the menu header is at the very front */

	background-color: rgba(0, 0, 0, 0.616);
	height: 60px;
	width: 100%;

	display: flex;
	justify-content: center;
	align-items: center;
}

a {
	color: white;
	text-decoration: none;
}

ul {
	color: white;
	list-style: none;
	width: 100vw;

	display: flex;
	justify-content: center;
	align-items: center;
	gap: 10%;
}

ul li {
	font-size: 1.2rem;
	cursor: pointer;
	padding: 4px;
	border: 2px solid transparent;

	transition: 150ms ease-in-out;
}

ul li:hover {
	border-bottom: 2px solid white;
}

@media (max-width: 875px) {
	ul {
		padding: 0;
	}

	/* Make hamburger menu */
}
</style>

