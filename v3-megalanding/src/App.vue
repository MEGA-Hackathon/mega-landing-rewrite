<template>
	<HomePage />
	<SignupPage />
</template>

<script>
import HomePage from './components/HomePage.vue';
import SignupPage from './components/SignupPage.vue';

export default {
	name: "App",
	components: {
		HomePage,
		SignupPage,
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
