<script module>
	import { defineMeta } from '@storybook/addon-svelte-csf'
	import Button from '$lib/atoms/Button.svelte'

	const { Story } = defineMeta({
		title: 'Atoms/Button',
		component: Button,
		parameters: {
			layout: 'centered'
		}
	})
</script>

<Story name="Default" args={{ label: 'Button' }} />
