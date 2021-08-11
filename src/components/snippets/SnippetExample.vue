<template>
	<div class="demo">
		<slot />
	</div>
</template>

<script>
export default {
	name: 'SnippetExample',
	setup() {
		return {};
	},
};
</script>

<style lang="scss" scoped>
.demo {
	padding: 1.5rem;
}
</style>
