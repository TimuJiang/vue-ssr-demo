<template lang='pug'>
	.m-header
		.m-logo
			img(src="~assets/images/logo.png")
		ul.m-menu
			nuxt-link( to="/car/type")
				li.m-menu-item  车型总览
			nuxt-link( to="/car/type")
				li.m-menu-item  车型总览
			nuxt-link( to="/register")
				li.m-menu-item  车型总览
</template>

<script>
	export default {
		name: 'm-header',

	}
</script>
<style lang="scss" scoped>
	.m-header {
		img {
			height: 50px;
		}
	}
</style>
