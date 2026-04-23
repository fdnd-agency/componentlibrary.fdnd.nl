<script>
	import { greet } from '$lib/vitest-examples/greet.js'

	/**
	 * @typedef {Object} Props
	 * @property {{name: string}} host The host name string
	 * @property {{name: string}} guest The guest name string
	 */

	/** @type {Props} */
	const { host = 'SvelteKit', guest = 'Vitest', ...props } = $props()
</script>

<h1>{greet(host)}</h1>
<p>{greet(guest)}</p>
