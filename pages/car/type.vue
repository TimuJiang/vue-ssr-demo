<template lang='pug'>
	.type
		span xxxxxxxx
</template>

<script>
	export default {
		name: 'type',
		async asyncData({$axios}) {
			$axios.$get('/product/listCarOverview')
				.then(result => {
					return result
				})
				.catch(error => {
					return error
				})
		}
	}
</script>
<style lang="scss" scoped>

</style>
