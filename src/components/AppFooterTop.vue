<script>
export default {
	data() {
		return {
			comicsLinks: [`Characters`, `Comics`, `Movies`, `Tv`, `Games`, `Videos`, `News`],
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
			shopLinks: [`Shop DC`, `Shop DC Collectibles`],
		};
	},
};
</script>

<template>
	<div class="row">
		<div class="col-6 deb">
			<div class="row text-white">
				<div class="col-3 deb pe-0">
					<span class="fs-6 fw-bold">DC COMICS</span>

					<ul class="p-0 mt-2">
						<li v-for="link in comicsLinks" class="list-group-item text-white-50 lh-base">
							{{ link }}
						</li>
					</ul>
				</div>

				<div class="col-2 deb px-0">
					<span class="fs-6 fw-bold">DC</span>

					<ul class="p-0 mt-2">
						<li v-for="link in dcLinks" class="list-group-item text-white-50">
							{{ link }}
						</li>
					</ul>
				</div>

				<div class="col-2 deb px-0">
					<span class="fs-6 fw-bold">SITES</span>

					<ul class="p-0 mt-2">
						<li v-for="link in sitesLinks" class="list-group-item text-white-50">
							{{ link }}
						</li>
					</ul>
				</div>
			</div>
		</div>
		<div class="col-6 deb text-end">
			<img src="../assets/dc-logo-bg.png" />
		</div>
	</div>
</template>

<style scoped></style>
