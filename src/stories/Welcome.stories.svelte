<script module>
	import { defineMeta } from '@storybook/addon-svelte-csf'
	import { Welcome } from '$lib'
	// import { fn } from 'storybook/test'

	const { Story } = defineMeta({
		title: 'Vitest/Welcome',
		component: Welcome
	})
</script>

<Story name="Primary" />
