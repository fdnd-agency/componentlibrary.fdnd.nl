<section class="intro">
<article>
	<h2 class="large-heading">Frontender worden?</h2>
	<p class="xlarge-body">FDND is de enige tweejarige hbo-opleiding voor frontend in Nederland.</p>
	<p class="medium-body">
            Wil jij websites ontwerpen én bouwen? Bij FDND leer je in twee jaar hoe je dat doet, zodat je snel aan de slag kunt in het werkveld.
            Je werkt met de nieuwste technieken om websites te bouwen en ontwikkelt belangrijke skills zoals samenwerken, communiceren en je tijd inschatten.
        </p>
		<p class="medium-body">
                        Tijdens de opleiding werk je aan echte projecten voor echte opdrachtgevers, zoals Funda, Schiphol en de Openbare
            Bibliotheek van Amsterdam (OBA). Ook werk je samen met bekende bureaus zoals De Voorhoede en HyperSolid.
        </p>
	<a href="/" class="button">Loop een ochtend met ons mee</a>
	<figure>
		<img src="/funda-fdnd.jpg" alt="Lars Schuitema, werkzaam als developer bij Funda geeft feedback aan studenten" />
		<figcaption class="large-body">Sprint review <br> Funda</figcaption>
	</figure>
</article>
</section>

<style>
	.intro {
		background-color: var(--base-color);
	}

	article {
		background-color: var(--background);
		padding: 2rem var(--padding-side);
		isolation: isolate;
		display: flex;
		flex-direction: column;
		gap: 1.1rem;

		@media (min-width: 768px) {
			display: grid;
			grid-template-columns: 1fr 1fr;
			grid-template-rows: 0fr 0fr;
			padding: 4rem var(--padding-side);
			column-gap: 3rem;
		}

		@media (min-width: 1024px) {
			padding: var(--padding-side) var(--padding-side) 0 calc(var(--padding-side) * 2);
			margin-bottom: 16rem;
			margin-top: 1rem;
			grid-template-columns: 0.85fr 1fr;
			column-gap: 3rem;
		}

		@media (min-width: 1440px) {
			padding-left: max(calc(var(--padding-side) * 2), calc((100% - 90rem) / 2 + calc(var(--padding-side) * 2)));
			padding-right: max(var(--padding-side), calc((100% - 90rem) / 2 + var(--padding-side)));
			margin-bottom: 5rem;
		}
	}

	h2, p, a.button {
		@media (min-width: 768px) {
			grid-column: 2;
		}
	}

	p {
		@media (min-width: 1024px) { 
			max-width: 42ch;
		}
	}

	a.button {
		@media (min-width: 1024px) {
			justify-self: start;
		}
	}

	a.button {
		background: var(--yellow);
		align-self: flex-start;
	}

	a.button::after {
		background: var(--yellow);
	}

	figure {
		position: relative;

		@media (min-width: 768px) {
			grid-column: 1;
			grid-row: 1 / -1;
			align-self: start;
		}

		@media (min-width: 1024px) {
			align-self: start;
		}
	}

	img {
		/* width: 100%; */
		border-radius: 1.5rem;

		@media (min-width: 768px) and (max-width: 1023px) {
			max-height: 28rem;
			object-fit: cover;
		}

		@media (min-width: 1024px) {
			height: 40rem;
			object-fit: cover;
		}

	}

	figcaption {
		position: absolute;
		bottom: 0;
		left: -0.5rem;
		transform: translateY(50%);
		background-color: var(--background);
		border: 2px solid var(--color);
		border-radius: var(--small-radius);
		padding: 0.25rem 0.75rem;
	}
</style>