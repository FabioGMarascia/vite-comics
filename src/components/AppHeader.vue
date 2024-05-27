<script>
import NavBar from "./AppHeaderComponents/NavBar.vue";
import Jumbotrone from "./AppHeaderComponents/Jumbotrone.vue";

export default {
	name: "AppHeader",
	components: {
		NavBar,
		Jumbotrone,
	},
	data() {
		return {};
	},
};
</script>

<template>
	<div class="container">
		<NavBar />
	</div>
	<Jumbotrone />
</template>

<style scoped></style>
