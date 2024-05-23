<script>
export default {
	data() {
		return {
			cards: [
				{
					title: `DIGITAL COMICS`,
					src: `../assets/buy-comics-digital-comics.png`,
				},
				{
					title: `DC MERCHANDISE`,
					src: `../assets/buy-comics-merchandise.png`,
				},
				{
					title: `SUBSCRIPTION`,
					src: `../assets/buy-comics-subscription.png`,
				},
				{
					title: `COMIC SHOP LOCATOR`,
					src: `../assets/buy-comics-shop-locator.png`,
				},
				{
					title: `DC POWER VISA`,
					src: `../assets/buy-dc-power-visa.svg`,
				},
			],
		};
	},
	mounted() {
		console.log(this.cards[0].src);
	},
};
</script>

<template>
	<div class="row py-5 deb justify-content-center px-5">
		<div v-for="card in cards" class="col deb mx-1">
			<div class="row">
				<div class="col-4 px-0">
					<img :src="card.src" />
				</div>

				<div class="col-8 px-0 fw-bold text-white my-auto ps-1">
					<span>{{ card.title }}</span>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
img {
	width: 100%;
}
</style>
