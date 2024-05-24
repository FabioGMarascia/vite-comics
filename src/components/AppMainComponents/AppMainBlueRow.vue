<script>
export default {
	name: "AppMainBlueRow",
	data() {
		return {
			cards: [
				{
					title: `DIGITAL COMICS`,
					src: `buy-comics-digital-comics.png`,
				},
				{
					title: `DC MERCHANDISE`,
					src: `buy-comics-merchandise.png`,
				},
				{
					title: `SUBSCRIPTION`,
					src: `buy-comics-subscriptions.png`,
				},
				{
					title: `COMIC SHOP LOCATOR`,
					src: `/buy-comics-shop-locator.png`,
				},
				{
					title: `DC POWER VISA`,
					src: `buy-dc-power-visa.svg`,
				},
			],
		};
	},
	methods: {
		getImg(path) {
			let risultato = new URL(`../../assets/` + path, import.meta.url);
			return risultato.href;
		},
	},
};
</script>

<template>
	<div class="row py-5 justify-content-center">
		<div v-for="card in cards" class="col-2 mx-3 px-0">
			<div class="d-flex h-100 text-end">
				<div class="col-4 px-0 my-auto deb">
					<img :src="getImg(card.src)" class="img-fluid" />
				</div>

				<div class="col-8 px-0 fw-bold text-white my-auto text-center deb">
					<span class="my-fs">{{ card.title }}</span>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
img {
	height: 4rem;
}

.my-fs {
	font-size: 0.76rem;
}
</style>
