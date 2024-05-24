<script>
import AppMainContent from "./AppMainComponents/AppMainContent.vue";
import AppMainBlueRow from "./AppMainComponents/AppMainBlueRow.vue";

export default {
	components: {
		AppMainContent,
		AppMainBlueRow,
	},
};
</script>

<template>
	<div class="mainContentBox bg-black">
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
.mainBlueRowBox {
	background-color: #0282f9;
}
</style>
