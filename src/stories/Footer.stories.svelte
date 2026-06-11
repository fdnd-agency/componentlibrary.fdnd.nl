<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf'
  import Footer from '$lib/organisms/Footer.svelte'

  const { Story } = defineMeta({
    title: 'Organisms/Footer',
    component: Footer,
    parameters: {
      layout: 'fullscreen'
    }
  })
</script>

<Story name="Default" />