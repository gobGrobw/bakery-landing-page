<script setup>
defineProps({
	bgColor: {
		type: String,
		required: true,
	},
	id: {
		type: String,
		required: true,
	},
});
</script>

<template>
	<div class="body" v-bind:id="id">
		<slot name="title"></slot>
		<div id="products">
			<slot name="product"></slot>
		</div>
	</div>
</template>

<style scoped>
.body {
	background-color: v-bind(bgColor);
	height: 80vh;
	text-align: center;

	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;

	overflow: hidden;
}

#products {
	display: grid;
	grid-auto-flow: column;
	gap: 5vw;
	margin-top: 80px;
}

@media (max-width: 815px) {
	.body {
		height: auto;
	}

	#products {
		margin-top: 20px;
		grid-auto-flow: dense;
		gap: 10px;
		margin-bottom: 20px;
	}
}
</style>

