<script>
export default {
	data() {
		return {
			cards: [
				{
					title: `DIGITAL COMICS`,
					src: `/src/assets/buy-comics-digital-comics.png`,
				},
				{
					title: `DC MERCHANDISE`,
					src: `/src/assets/buy-comics-merchandise.png`,
				},
				{
					title: `SUBSCRIPTION`,
					src: `/src/assets/buy-comics-subscriptions.png`,
				},
				{
					title: `COMIC SHOP LOCATOR`,
					src: `/src/assets/buy-comics-shop-locator.png`,
				},
				{
					title: `DC POWER VISA`,
					src: `/src/assets/buy-dc-power-visa.svg`,
				},
			],
		};
	},
};
</script>

<template>
	<div class="row py-5 justify-content-center">
		<div v-for="card in cards" class="col-2 mx-3 deb px-0">
			<div class="row text-center deb mx-0 align-items-center">
				<div class="col-4 px-0">
					<img :src="card.src" class="my-auto" />
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
	width: 3rem;
	height: 100%;
}
</style>
