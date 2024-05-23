<script>
import AppMainContent from "./AppMainContent.vue";
import AppMainBlueRow from "./AppMainBlueRow.vue";

export default {
	components: {
		AppMainContent,
		AppMainBlueRow,
	},
};
</script>

<template>
	<div class="mainContentBox deb bg-black">
		<div class="container">
			<AppMainContent />
		</div>
	</div>

	<div class="mainBlueRowBox deb">
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
