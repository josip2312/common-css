<template>
	<section class="section buttons" id="buttons">
		<h2 class="h2 section-title">Buttons</h2>
		<div class="example">
			<TabExpander :snippet="snippet" />
			<SnippetExample>Example</SnippetExample>
		</div>
	</section>
</template>

<script>
export default {
	name: 'SnippetButton',
	setup() {
		const snippet = `.name { color: red; }`;

		return { snippet };
	},
};
</script>

<style lang="scss" scoped>
.example {
	border: 0.2rem solid var(--text2);
	border-radius: var(--br-md);
}
</style>
