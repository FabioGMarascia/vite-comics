<script>
export default {
	data() {
		return {
			comicsLinks: [`Characters`, `Comics`, `Movies`, `Tv`, `Games`, `Videos`, `News`],
			shopLinks: [`Shop DC`, `Shop DC Collectibles`],
			dcLinks: [
				`Terms Of Use`,
				`Privacy policy (New)`,
				`Ad Choices`,
				`Advertising`,
				`Jobs`,
				`Subscriptions`,
				`Talent Workshops`,
				`CPSC Certificates`,
				`Ratings`,
				`Shop Help`,
				`Contact Us`,
			],
			sitesLinks: [`DC`, `MAD Magazine`, `DC Kids`, `DC Universe`, `DC Power Vista`],
		};
	},
};
</script>

<template>
	<div class="row justify-content-between">
		<div class="col-6">
			<div class="row text-white pt-5 ps-3">
				<div class="col-2 px-0">
					<span class="fs-6 fw-bold">DC COMICS</span>

					<ul class="p-0 mt-2">
						<li v-for="link in comicsLinks" class="list-group-item text-white-50 lh-base">
							{{ link }}
						</li>
					</ul>

					<span class="fs-6 fw-bold">SHOP</span>

					<ul class="p-0 mt-2">
						<li v-for="link in shopLinks" class="list-group-item text-white-50 lh-base">
							{{ link }}
						</li>
					</ul>
				</div>

				<div class="col-2 px-0 mx-3">
					<span class="fs-6 fw-bold">DC</span>

					<ul class="p-0 mt-2">
						<li v-for="link in dcLinks" class="list-group-item text-white-50">
							{{ link }}
						</li>
					</ul>
				</div>

				<div class="col-2 px-0">
					<span class="fs-6 fw-bold">SITES</span>

					<ul class="p-0 mt-2">
						<li v-for="link in sitesLinks" class="list-group-item text-white-50">
							{{ link }}
						</li>
					</ul>
				</div>
			</div>
		</div>

		<div class="col-5 footerTopRight deb text-end"></div>
	</div>
</template>

<style scoped>
.footerTopRight {
	background-image: url(../assets/dc-logo-bg.png);
	background-size: cover;
	background-position: center;
	height: 22rem;
}
</style>
