<script>
	let { label, onclick, class: className = '', ...props } = $props()
</script>

<button type="button" class={['button', 'small-body', className].filter(Boolean).join(' ')} {onclick} {...props}>
	{label}
</button>

<style>
	.button {
		display: inline-flex;
		align-items: center;
		justify-content: center;
		cursor: pointer;
		position: relative;
		background: var(--background);
		border: 1px solid var(--color);
		border-radius: var(--small-radius);
		padding: 0.75em 1.5em;
		letter-spacing: 0.05em;
		font-weight: 550;
		color: var(--color);
		top: 0;
		transition: top 0.1s ease-out;
	}

	.button::after {
		content: '';
		width: 100%;
		height: 100%;
		position: absolute;
		left: -4px;
		bottom: -4px;
		background: var(--background);
		border: 1px solid currentColor;
		border-radius: 0.5rem;
		z-index: -1;
		transition: transform 0.1s ease-out;
	}

	.button:hover {
		top: 1px;
	}

	.button:hover::after {
		transform: translate(1px, -1px);
	}
</style>
