<script>
	import CreatingTomorrow from '$lib/icons/CreatingTomorrow.svelte'
</script>

<footer class="footer">
	<h2 class="medium-heading">FDND microsite</h2>
	<p class="large-body description">FDND maakt gebruik van microsites. Microsites zijn kleine websites ter ondersteuning van een campagne, informatie over een product, dienst of voor een ander specifiek doel.</p>

	<nav class="footer-nav">
		<ul>
			<li><a href="https://fdnd.nl" class="button medium-body">FDND.nl</a></li>
			<li><a href="https://contact.fdnd.nl/" class="button medium-body">Contact & routebeschrijving</a></li>
			<li><a href="https://programma.fdnd.nl/" class="button medium-body">Programma</a></li>
			<li><a href="https://partners.fdnd.nl/" class="button medium-body">Partners</a></li>
			<li><a href="https://niveaumatrix.fdnd.nl/" class="button medium-body">Niveau-matrix</a></li>
			<li><a href="https://docs.fdnd.nl/" class="button medium-body">Documenten</a></li>
		</ul>
	</nav>

	<CreatingTomorrow />
	<p class="hosting small-body">FDND relies on hosting provided by <a href="https://www.netlify.com">netlify</a></p>
</footer>

<style>
	.footer {
		background-color: var(--base-color);
		color: var(--blue);
		padding: 4rem var(--padding-side);
		display: flex;
		flex-direction: column;
		gap: 1.5rem;
	}

	@media (min-width: 1024px) {
		.footer {
			display: grid;
			grid-template-columns: fit-content(var(--max-width));
			justify-content: center;
		}
	}

	h2 {
		color: var(--blue);
	}

	.description {
		color: var(--blue);
		max-width: 36rem;
		margin-top: 0;
	}

	.footer-nav ul {
		list-style: none;
		padding: 0;
		display: flex;
		flex-wrap: wrap;
		gap: 1rem;
		isolation: isolate;
	}

	.footer-nav a {
		font-weight: 550;
		letter-spacing: 0.05em;
	}

</style>