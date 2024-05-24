<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
	name: "App",
	components: {
		AppHeader,
		AppMain,
		AppFooter,
	},
	data() {
		return {};
	},
};
</script>

<template>
	<header>
		<div class="container">
			<AppHeader />
		</div>
	</header>

	<main>
		<AppMain />
	</main>

	<footer>
		<AppFooter />
	</footer>
</template>

<style scoped></style>
