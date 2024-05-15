<template>
	<div id="container">
		<div id="wrapper">
			<div class="image image-1"></div>
			<div class="image image-2"></div>
			<div class="image image-3"></div>
		</div>
		<slot></slot>
	</div>
</template>

<style scoped>
#container {
	height: 100vh;
	width: 100vw;
}

.image {
	position: absolute;
	z-index: -1;
	height: 100%;
	width: 100%;
}

.image-1 {
	background: url('./images/background-1.jpg');
	background-repeat: no-repeat;
	background-position: center;
	background-size: cover;
}
</style>

