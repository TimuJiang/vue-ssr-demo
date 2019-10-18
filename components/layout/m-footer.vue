<template lang="pug">
	.m-footer
		.m-footer__content
			.m-footer__content-item
				.title 品牌天地
				ul
					li
						a 集团概述
		.m-footer__copyright
			.left
				p © 2013 浙江吉利控股集团 浙ICP备11045738号-8
				p
					img(src="https://dm30-dev.obs.myhwclouds.com/GeelyOfficial/Files/Common/Footer/logo.png")
					|  中国互联网诚信示范单位
			.right
				p 400-886-9888
				p

</template>

<script>
    export default {
        name: "m-footer"
    }
</script>

<style lang="scss" scoped>
	.m-footer {
		background-color: #055a94;
		padding: 10px 0;
		color: #FFFFFF;
		&__content {
			width: 1200px;
			margin: 0 auto;
		}
		&__copyright {
			width: 1200px;
			margin: 0 auto;
		}
	}
</style>
