<script>
	import '$lib/assets/style.css'
	import { Header } from '$lib'

	let { children, data } = $props()
</script>

<Header />

<main>
	{@render children()}
</main>
