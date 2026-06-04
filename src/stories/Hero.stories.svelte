<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf'
  import Hero from '$lib/organisms/Hero.svelte'

  const { Story } = defineMeta({
    title: 'Organisms/Hero',
    component: Hero,
    parameters: {
      layout: 'fullscreen'
    }
  })
</script>

<Story
  name="Default"
  args={{
    label: 'Associate Degree',
    title: 'Frontend Design & Development',
    image: '/herostudenten-image-fdnd.jpg',
    imageAlt: 'Studenten van FDND',
    duration: 'Twee jaar',
    type: 'Voltijd',
    openAvond: '9 juni 2026'
  }}
/>
