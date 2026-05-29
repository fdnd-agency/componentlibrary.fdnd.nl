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
