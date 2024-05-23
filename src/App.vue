<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
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
	<header class="deb">
		<div class="container">
			<AppHeader />
		</div>
	</header>

	<div class="container">
		<AppMain />
		<AppFooter />
	</div>
</template>

<style scoped></style>
