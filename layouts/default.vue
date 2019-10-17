<template lang="pug">
	.default-layout
		m-header
		nuxt
		m-footer
</template>

<script>
	import MHeader from '~/components/layout/m-header'
	import MFooter from '~/components/layout/m-footer'
	export default {
		components: { MHeader, MFooter },
		data() {
			return {
				clipped: false,
				drawer: false,
				fixed: false,
				items: [
					{
						icon: 'mdi-apps',
						title: 'Welcome',
						to: '/'
					},
					{
						icon: 'mdi-chart-bubble',
						title: 'Inspire',
						to: '/inspire'
					}
				],
				miniVariant: false,
				right: true,
				rightDrawer: false,
				title: 'Vuetify.js'
			}
		}
	}
</script>
