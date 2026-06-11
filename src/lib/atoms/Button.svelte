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
	}

.button:hover {
		opacity: 0.8;
	}
</style>
