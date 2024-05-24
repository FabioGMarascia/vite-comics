<script>
import ComicsList from "./MainContentComponents/ComicsList.vue";

export default {
	name: "AppMainContent",
	components: {
		ComicsList,
	},
	data() {
		return {};
	},
};
</script>

<template>
	<ComicsList class="py-5" />
</template>

<style scoped></style>
