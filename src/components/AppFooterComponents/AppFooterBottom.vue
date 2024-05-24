<script>
export default {
	data() {
		return {
			icons: [
				`footer-facebook.png`,
				`footer-twitter.png`,
				`footer-youtube.png`,
				`footer-pinterest.png`,
				`footer-periscope.png`,
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
	<div class="row py-5 text-white">
		<div class="col-6">
			<button class="btn border border-2 border-primary text-white rounded-0">
				SIGN-UP NOW!
			</button>
		</div>

		<div class="col-6">
			<div class="row">
				<div class="col-7 text-end px-0 my-auto">
					<span class="fw-bold fs-5 my-blue"> FOLLOW US </span>
				</div>

				<div class="col-5 px-0">
					<div class="d-flex justify-content-end">
						<img v-for="icon in icons" :src="getImg(icon)" class="mx-2" />
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
img:hover {
	cursor: pointer;
}

.my-blue {
	color: #0282f9;
}
</style>
