<script>
	let { label, title, image, imageAlt = '', duration, type, openAvond, badge, badgeAlt = '' } = $props()
</script>

<section class="hero">
	<article class="card">
		<hgroup class="card-content">
			<p class="subtitle medium-body">{label}</p>
			<h1 class="xlarge-heading">{title}</h1>
		</hgroup>
		<figure class="image-wrapper">
			<img src={image} alt={imageAlt} />
			{#if badge}
				<img class="badge" src={badge} alt={badgeAlt} />
			{/if}
		</figure>
		<dl class="opleiding-info">
			<dt class="medium-body">Duur</dt>
			<dd class="small-body">{duration}</dd>
			<dt class="medium-body">Type</dt>
			<dd class="small-body">{type}</dd>
			<dt class="medium-body">Open avond</dt>
			<dd class="small-body">{openAvond}</dd>
		</dl>
	</article>
</section>

<style>
	.hero {
		background-color: var(--base-color);
		padding-left: var(--radius);
		padding-right: var(--radius);
	}

	.card {
		background-color: var(--background);
		border-radius: 1.5rem 1.5rem 0 0;

		@media (min-width: 768px) {
			position: relative;
			border-radius: 1.5rem 0 0 0;
		}
	}

	.card-content {
		padding: var(--padding-side) 1.5rem 0;
		background-color: var(--background);
		border-radius: var(--section-width);

		@media (min-width: 768px) {
			position: absolute;
			z-index: 1;
			top: 1.5em;
			right: 0;
			padding: 0 1.5rem 1.5rem;
			border-radius: 0 0 0 var(--radius);
			width: 26rem;


		@media (min-width: 1024px) {
			padding: 0 clamp(1.5rem, calc(100vw / 24 * 40 / 60), 2.5rem) clamp(1.5rem, calc(100vw / 24 * 40 / 60), 2.5rem);
			width: 49%;
		}
	}

	.subtitle {
		color: var(--blue);
		text-transform: uppercase;
		font-weight: 700;
		letter-spacing: 0.05em;
	}

	h1 {
		color: var(--blue);
	}

	.image-wrapper {
		position: relative;
		padding: var(--padding-side) var(--padding-side) 0;
	}

	.image-wrapper img:first-child {
		width: 100%;
		border-radius: 1.5rem;
		min-height: 25rem;
		object-fit: cover;
	}

	.badge {
		position: absolute;
		bottom: -1rem;
		right: -0.5rem;
		width: 6rem;
	}

	.opleiding-info {
		display: grid;
		grid-template-rows: auto auto;
		grid-auto-flow: column;
		grid-auto-columns: max-content;
		gap: 0 2rem;
		padding: 0.75rem 1.5rem 1.5rem;

		@media (min-width: 768px) {
			position: absolute;
			bottom: 0;
			left: 0;
			z-index: 1;
			background-color: var(--background);
			padding: 1rem 1.5rem 1.5rem 2rem;
			border-radius: 0 var(--radius) 0 0;
			gap: 0 1.5rem;
			width: 21em;

			dt {

		@media (min-width: 1024px) {
			padding: 1.5rem 2rem 2rem 3.5rem;
			gap: 0 2rem;
			width: 36%;
		}
	}

	dt {
		font-weight: 700;
		text-transform: uppercase;
		letter-spacing: 0.05em;
		color: var(--blue);
	}

	dd {
		color: var(--blue);
		text-transform: uppercase;
	}
</style>
