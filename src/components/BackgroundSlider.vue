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
	background: url('../images/background-1.jpg');
	background-repeat: no-repeat;
	background-position: center;
	background-size: cover;
	width: 100vw;
}

.image-2 {
	background: url('./images/background-2.jpg');
	background-repeat: no-repeat;
	background-position: center;
	background-size: cover;
	width: 100vw;
}

.image-3 {
	background: url('./images/background-3.jpg');
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

