<template>
	<m-header></m-header>
</template>

<script>
	import MHeader from '../components/layout/m-header'
	export default {
		components: { MHeader },
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
