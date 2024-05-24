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
		<div v-for="card in cards" class="col-2 mx-3 px-0">
			<div class="d-flex h-100 text-end">
				<div class="col-4 px-0 my-auto">
					<img :src="card.src" class="img-fluid" />
				</div>

				<div class="col-8 px-0 fw-bold text-white my-auto text-center">
					<span>{{ card.title }}</span>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
img {
	height: 4rem;
}
</style>
