<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf'
  import Main from '$lib/organisms/Main.svelte'
  import Intro from '$lib/organisms/Intro.svelte'

  const { Story } = defineMeta({
    title: 'Organisms/Main',
    component: Main,
    parameters: {
      layout: 'fullscreen'
    }
  })
</script>

<Story name="Default">
  {#snippet children()}
    <Intro />
  {/snippet}
</Story>