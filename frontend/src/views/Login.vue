<template>
<v-layout column align-center>
	<v-layout wrap justify-space-around>
		<h2 class="mb-2">Login Form</h2>
	</v-layout>
	<v-form class="login-form">
	  <v-text-field
		label="E-mail"
		required
	  ></v-text-field>

	  <v-text-field
		label="Password"
		required
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

<style lang="stylus" scoped>
	.login-form
		min-width 300px
		max-width 400px
		width 20%
</style>

