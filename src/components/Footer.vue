<template>
	<div class="body">
		<div id="left">
			<h2>Doe's Delight</h2>
			<h4>A bite with a thousand flavours</h4>
		</div>

		<div id="border"></div>

		<div id="right">
			<h2>Contact Us!</h2>
			<ul>
				<li>fakeEmail@gmail.com</li>
				<li>+1234-456-890</li>
			</ul>
		</div>
	</div>
</template>

<style scoped>
.body {
	height: 15vh;
	background-color: rgb(227, 188, 132);
	width: 100%;
	display: flex;
	justify-content: space-around;
	align-items: center;
	padding: 0 30% 0 30%;
}

#border {
	width: 2px;
	height: 100px;
	border: 2px solid rgb(37, 37, 37);
}

h2 {
	font-family: cursive;
	font-size: 2rem;
}

h4 {
	font-weight: lighter;
	font-family: 'Times New Roman', Times, serif;
	font-size: 1.4rem;
}

ul {
	list-style: none;
	padding: 0;
}

ul li {
	font-size: 1.1rem;
}

@media (max-width: 1250px) {
	.body {
		padding: 0;
		display: flex;
		padding: 5px;
	}

	#left,
	#right {
		text-align: center;
	}

	#border {
		margin: 0 5px 0 5px;
	}

	h2 {
		font-size: 1.5rem;
	}

	h4 {
		font-size: 1.2rem;
	}
}
</style>

