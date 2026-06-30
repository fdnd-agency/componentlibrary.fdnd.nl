<aside class="cta">
	<div class="cta-inner">
		<p class="subtitle small-body">Wil jij bij ons studeren?</p>
		<a href="https://www.hva.nl/opleidingen/ad-frontend-design-and-development" class="button small-body">Meer info op de HvA site</a>
	</div>
</aside>

<style>
	@keyframes up {
		to { transform: translateY(0); }
	}

	aside.cta {
		position: fixed;
		bottom: 0;
		right: var(--radius);
		z-index: 1;

		@media (min-width: 768px) {
			bottom: var(--radius);
		}
	}

	.cta-inner {
		padding: 1.5rem 1.75rem 1.75rem 1.5rem;
		display: flex;
		flex-direction: column;
		gap: 0.3rem;
		align-items: flex-start;
		background-color: var(--base-color);
		border-radius: var(--radius) 0 0 0;
		transform: translateY(100%);
		animation: up 0.4s 0.4s ease-out forwards;

		&::before {
			content: '';
			position: absolute;
			width: calc(var(--radius) * 2);
			height: calc(var(--radius) * 2);
			top: calc(var(--radius) * -2);
			right: 0;
			border-radius: 50%;
			box-shadow: var(--radius) var(--radius) 0 0 var(--base-color);
		}

		@media (min-width: 768px) {
			&::after {
				content: '';
				position: absolute;
				width: calc(var(--radius) * 2);
				height: calc(var(--radius) * 2);
				bottom: 0;
				left: calc(var(--radius) * -2);
				border-radius: 50%;
				box-shadow: var(--radius) var(--radius) 0 0 var(--base-color);
			}
		}
	}

	.subtitle {
		color: var(--background);
		text-transform: uppercase;
		font-weight: 700;
		letter-spacing: 0.05em;
	}

	a.button {
		background: var(--green);
	}

	a.button::after {
		background: var(--green);
	}
</style>