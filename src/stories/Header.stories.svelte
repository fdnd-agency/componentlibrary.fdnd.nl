<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf'
  import Header from '$lib/organisms/Header.svelte'

  const { Story } = defineMeta({
    title: 'Organisms/Header',
    component: Header,
    parameters: {
      layout: 'fullscreen'
    }
  })
</script>

<Story name="Default" />
