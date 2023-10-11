<template>
	<HomePage />
  <SponsorsComponent />
	<SignupPage />
</template>

<script>
import HomePage from './components/HomePage.vue';
import SignupPage from './components/SignupPage.vue';
import SponsorsComponent from './components/SponsorsComponent.vue';

export default {
	name: "App",
	components: {
		HomePage,
		SignupPage,
    SponsorsComponent
	},
};
</script>

<style>
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
	max-width: 100%;
	overflow: hidden;
}
</style>
