<script>
export default {
	name: "ComicsListCard",
	props: ["element"],
	data() {
		return {};
	},
};
</script>

<template>
	<div class="col-2 card-box px-3 py-4">
		<div class="img-box">
			<img :src="element.thumb" />
		</div>

		<div class="card-name mt-3 text-uppercase">{{ element.series }}</div>
	</div>
</template>

<style scoped>
.card-name {
	color: white;
	font-size: 0.8rem;
}

img {
	width: 100%;
	height: 18rem;
	object-fit: center;
}

.img-box {
	height: 12rem;
	overflow: hidden;
}
</style>
