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
	<div class="footerTopBox">
		<div class="container">
			<AppFooterTop />
		</div>
	</div>

	<div class="footerBottomBox">
		<div class="container">
			<AppFooterBottom />
		</div>
	</div>
</template>

<style scoped>
.footerTopBox {
	background-image: url(../assets/footer-bg.jpg);
	background-size: cover;
	height: 22rem;
}

.footerBottomBox {
	background-color: #303030;
}
</style>
