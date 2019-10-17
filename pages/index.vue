<template lang="pug">
	v-layout( column justify-center align-center)
		m-banner
		v-flex(xs12 sm8 md6)
			v-card
				v-card-title.headline
				v-card-text
					p Vuetify is a progressive Material Design component framework for Vue.js. It was designed to empower developers to create amazing applications.
					p
						span For more information on Vuetify, check out the
						a( href="https://vuetifyjs.com" target="_blank")
						span documentation
					p
						| If you have questions, please join the official
						a(href="https://chat.vuetifyjs.com/" target="_blank" title="chat")
						| discord
						|.
					p
						| Find a bug? Report it on the github
						a(href="https://github.com/vuetifyjs/vuetify/issues" target="_blank" title="contribute")
						| issue board
						|.
					p
						| Thank you for developing with Vuetify and I look forward to bringing more exciting features in the future.
					.text-xs-right
				v-card-actions
					v-spacer
					v-btn( color="primary" nuxt to="/inspire" ) Continue
</template>

<script>
    import MBanner from '~/components/m-banner'
	export default {
		components: {
            MBanner
		}
	}
</script>
