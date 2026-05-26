<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf'
  import Header from '$lib/molecules/Header.svelte'

  const { Story } = defineMeta({
    title: 'Molecules/Header',
    component: Header,
    parameters: {
      layout: 'fullscreen'
    }
  })
</script>

<Story name="Default" />
