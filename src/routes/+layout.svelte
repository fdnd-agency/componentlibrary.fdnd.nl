<script>
	import '$lib/assets/style.css'
	import { Header } from '$lib'

	let { children, data } = $props()
</script>

<svelte:head>
	<title>FDND Component Library</title>
</svelte:head>

<Header />

<main>
	{@render children()}
</main>
