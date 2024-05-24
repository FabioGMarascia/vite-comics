<script>
import AppMainContent from "./AppMainComponents/AppMainContent.vue";
import AppMainBlueRow from "./AppMainComponents/AppMainBlueRow.vue";

export default {
	name: "AppMain",
	components: {
		AppMainContent,
		AppMainBlueRow,
	},
};
</script>

<template>
	<div class="mainContentBox position-relative py-4">
		<div class="container">
			<AppMainContent />
		</div>
	</div>

	<div class="mainBlueRowBox">
		<div class="container">
			<AppMainBlueRow />
		</div>
	</div>
</template>

<style scoped>
.mainContentBox {
	background-color: #1c1c1c;
}

.mainBlueRowBox {
	background-color: #0282f9;
}
</style>
