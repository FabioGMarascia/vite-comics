<script>
import AppFooterTop from "./AppFooterTop.vue";
import AppFooterBottom from "./AppFooterBottom.vue";

export default {
	components: {
		AppFooterTop,
		AppFooterBottom,
	},
};
</script>

<template>
	<div class="footerTopBox deb">
		<div class="container">
			<AppFooterTop />
		</div>
	</div>

	<div class="footerBottomBox deb">
		<div class="container">
			<AppFooterBottom />
		</div>
	</div>
</template>

<style scoped>
.footerTopBox {
	background-image: url(../assets/footer-bg.jpg);
	background-size: cover;
}

.footerBottomBox {
	background-color: #303030;
}
</style>
