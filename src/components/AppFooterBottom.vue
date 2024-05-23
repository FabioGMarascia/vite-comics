<script>
export default {
	data() {
		return {
			icons: [
				`/src/assets/footer-facebook.png`,
				`/src/assets/footer-twitter.png`,
				`/src/assets/footer-youtube.png`,
				`/src/assets/footer-pinterest.png`,
				`/src/assets/footer-periscope.png`,
			],
		};
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
					<span class="fw-bold fs-5 text-primary"> FOLLOW US </span>
				</div>

				<div class="col-5 px-0">
					<div class="d-flex justify-content-end">
						<img v-for="icon in icons" :src="icon" class="mx-2" />
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
</style>
