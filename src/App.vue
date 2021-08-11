<template>
	<TheHeader />
	<main class="main container">
		<AppShowcase />
		<AppSnippets />
	</main>
</template>

<script>
export default {
	name: 'App',
};
</script>

<style lang="scss">
@use "./sass/main.scss";

.main {
	padding: 5vh clamp(1rem, 5vw, 3rem);
}
</style>
