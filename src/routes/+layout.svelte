<script>
	import '$lib/assets/style.css'
	import { Header, Main, Footer } from '$lib'

	let { children, data } = $props()
</script>

<svelte:head>
	<title>FDND Component Library</title>
</svelte:head>

<Header />
<Main>
	{@render children()}
</Main>
<Footer />