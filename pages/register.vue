<template lang='pug'>
	.register
		v-form(v-model="valid")
			v-container
				v-row
					v-text-field( v-model="firstName" :rules="_nameRules" :counter="10" label="请输入手机号码" required )
				v-row
					v-text-field( v-model="smsCode" :counter="6" label="请输入短信验证码" required )
				v-row
					v-text-field(type="password" v-model="password" :counter="20" label="请输入密码(至少6位数和字母组合)" required )
				v-row
					v-text-field(type="password" v-model="password2" :counter="20" label="请再次输入密码" required )
				v-row
					v-checkbox(v-model="agree" label="同意注册协议")
						v-icon(slot="append" ) mdi-mouse
</template>

<script>
	export default {
		data() {
			return {
				valid: false,
				project: 'default',
				firstName: '',
				smsCode: '',
				password: '',
				password2: '',
				agree: false,
				email: '',
			}
		},
		beforeCreate() {
			this._emailRules = [
				v => !!v || 'E-mail is required',
				v => /.+@.+/.test(v) || 'E-mail must be valid',
			]
			this._nameRules =  [
				v => !!v || 'Name is required',
				v => v.length <= 10 || 'Name must be less than 10 characters',
			]
		},
		asyncData(context) {
			return {project: 'nuxt'}
		}
	}
</script>
<style lang="scss" scoped>

</style>
