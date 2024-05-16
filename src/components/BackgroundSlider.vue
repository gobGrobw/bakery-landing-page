<template>
	<div id="container">
		<div id="wrapper">
			<div class="image image-1"></div>
			<div class="image image-2"></div>
			<div class="image image-3"></div>
			<div class="image image-1"></div>
		</div>
		<slot></slot>
	</div>
</template>

<style scoped>
#container {
	height: 100vh;
	width: 100vw;
}

#wrapper {
	display: flex;
	position: absolute;
}

.image {
	z-index: -1;
	height: 100vh;
	animation: slide 16s infinite;
	animation-fill-mode: forwards;
}

.image-1 {
	background: url('https://images.unsplash.com/photo-1469533778471-92a68acc3633?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
	background-repeat: no-repeat;
	background-position: center;
	background-size: cover;
	width: 100vw;
}

.image-2 {
	background: url('https://images.unsplash.com/photo-1666854859107-a14fbb69059a?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
	background-repeat: no-repeat;
	background-position: center;
	background-size: cover;
	width: 100vw;
}

.image-3 {
	background: url('https://images.unsplash.com/photo-1595526417596-c0fdbf75287b?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
	background-repeat: no-repeat;
	background-position: center;
	background-size: cover;
	width: 100vw;
}

@keyframes slide {
	0% {
		transform: translateX(0);
	}

	15% {
		transform: translateX(0);
	}

	30% {
		transform: translateX(-100%);
	}

	45% {
		transform: translateX(-100%);
	}

	60% {
		transform: translateX(-200%);
	}

	75% {
		transform: translateX(-200%);
	}

	90% {
		transform: translateX(-300%);
	}

	100% {
		transform: translateX(-300%);
	}
}
</style>

