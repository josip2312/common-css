<template>
	<section class="section buttons" id="buttons">
		<h2 class="h2">Inputs</h2>
		<TabExpander :snippet="snippet" />
	</section>
</template>

<script>
export default {
	name: 'SnippetInput',
	setup() {
		const snippet = `.input { color: blue; }`;

		return { snippet };
	},
};
</script>

<style lang="scss" scoped></style>
