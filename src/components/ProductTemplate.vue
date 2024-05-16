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
}

#products {
	display: grid;
	grid-template-columns: 1fr 1fr 1fr;
	grid-auto-flow: column;
	gap: 100px;
	margin-top: 80px;
}
</style>

