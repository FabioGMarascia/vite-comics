<script>
export default {
	name: "NavBar",
	data() {
		return {
			links: [
				{
					name: `CHARACTERS`,
					url: `#1`,
				},
				{
					name: `COMICS`,
					url: `#2`,
				},
				{
					name: `MOVIES`,
					url: `#3`,
				},
				{
					name: `TV`,
					url: `#4`,
				},
				{
					name: `GAMES`,
					url: `#5`,
				},
				{
					name: `COLLECTIBLES`,
					url: `#6`,
				},
				{
					name: `VIDEOS`,
					url: `#7`,
				},
				{
					name: `FANS`,
					url: `#8`,
				},
				{
					name: `NEWS`,
					url: `#9`,
				},
				{
					name: `SHOP`,
					url: `#10`,
				},
			],
		};
	},
};
</script>

<template>
	<div class="row my-3">
		<div class="col-3 my-auto">
			<img src="../../assets/dc-logo.png" />
		</div>

		<div class="col-9 px-0 text-end my-auto">
			<a
				v-for="link in links"
				:href="link.url"
				class="mx-3 text-decoration-none fw-bold my-link">
				{{ link.name }}</a
			>
		</div>
	</div>
</template>

<style scoped>
img {
	width: 5rem;
}

a {
	font-size: 0.8rem;
	color: black;
	padding: 2.75rem 0;
}

.my-link:hover {
	color: #0282f9;
	border-bottom: 5px solid #0282f9;
}
</style>
