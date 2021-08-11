<template>
	<div class="tab">
		<details open>
			<summary class="expand">Expand for code</summary>
			<pre class="snippet language-css" v-if="isExpanded">
        <code>
          {{snippet}}
        </code>
    </pre>
		</details>
	</div>
</template>

<script>
import { ref, onMounted } from 'vue';
export default {
	name: 'TabExpander',
	props: {
		snippet: {
			type: String,
			required: true,
		},
	},
	setup() {
		const isExpanded = ref(true);

		onMounted(() => {
			Prism.highlightAll();
		});

		return {
			isExpanded,
		};
	},
};
</script>

<style lang="scss" scoped>
.tab {
	display: flex;
	flex-direction: column;
}
.expand {
	background-color: var(--surface1);
	position: relative;
	cursor: pointer;
	text-align: center;
	padding: 1rem;
	border-top-right-radius: var(--br-md);
	border-top-left-radius: var(--br-md);

	&::marker {
		color: var(--text1);
	}

	&::before {
		content: '';
		position: absolute;
		top: 50%;
		left: 0;

		transform: translateY(-50%);
	}
}

.snippet {
	padding: 0.5rem;
	margin: 0;
	border-radius: var(--br-md);
}
</style>
