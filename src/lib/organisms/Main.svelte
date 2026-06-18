<script>
	let { children } = $props()
</script>

<main class="main">
	{@render children()}
</main>

<style>
	.main {
		background-color: var(--background);
		border-radius: 0 0 1.5rem 1.5rem;
		padding-bottom: 3rem;
		margin: 0 calc(var(--radius)) calc(var(--radius));
	}
</style>