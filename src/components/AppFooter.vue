<script>
import AppFooterTop from "./AppFooterComponents/AppFooterTop.vue";
import AppFooterBottom from "./AppFooterComponents/AppFooterBottom.vue";

export default {
	name: "AppFooter",
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
