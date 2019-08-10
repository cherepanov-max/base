<template>
<v-layout align-center justify-center column class="full-page">
	<v-layout wrap justify-space-around>
		<h2 class="mb-2">Login Form</h2>
	</v-layout>
	<v-form class="login-form">
	  <v-text-field
		label="E-mail"
		:rules="loginRules"
		class="mb-4"
		validate-on-blur
	  ></v-text-field>

	  <v-text-field
		label="Password"
		type="password"
		:rules="passwordRules"
		class="mb-4"
		validate-on-blur
	  ></v-text-field>
	<v-layout wrap justify-space-between>
		<v-btn
		color="success"
	
		width='45%'
	  >
		Sign In
	  </v-btn>

	  <v-btn
		color="warning"
		width='45%'
	  >
		Sign Up
	  </v-btn>
	</v-layout>
	  
	</v-form>
  </v-layout>
</template>

<script>
	export default {
		name: 'App',
		components: {

		},
		data: () => ({
			passwordRules: [
				v => (v || '').length >= 6 || 'Поле не может быть короче 6 символов',
			],
			loginRules: [
				v => (v || '').length > 0 || 'Поле не может быть пустым',
				v => ((v || '').match(/@/) && (v || '').match(/\./)) || 'Значение должно быть электронной почтой'
			]
		}),
	};
</script>





<style lang="stylus" scoped>
	.login-form
		min-width 300px
		max-width 400px
		width 20%
	.full-page
		margin-top 15vh;
</style>

