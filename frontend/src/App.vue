<template>
	<v-app >
		<div>
			<v-toolbar>
				<v-toolbar-items>
					<v-btn text to="/">Home</v-btn>
					<v-btn text to="/login">Login</v-btn>
				</v-toolbar-items>
			</v-toolbar>
		</div>
		<div>
			<v-content>
				<v-container fluid> 
					<router-view></router-view>
				</v-container>
			</v-content>
		</div>
	</v-app>
</template>

<script>


export default {
  name: 'App',
  components: {

  },
  data: () => ({

  }),
};
</script>
