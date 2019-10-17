<template lang='pug'>
	.register register {{ project }}
</template>

<script>
	export default {
		data() {
			return {project: 'default'}
		},
		asyncData(context) {
			return {project: 'nuxt'}
		}
	}
</script>
<style lang="scss" scoped>

</style>
