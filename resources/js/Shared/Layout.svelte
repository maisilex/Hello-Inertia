<script>
  import { inertia } from '@inertiajs/inertia-svelte'

  export let title
</script>
  
<svelte:head>
  <title>{$title ? `${$title} - Awesome App` : 'Awesome App'}</title>
</svelte:head>
  
<main>
  <header>
    <a use:inertia href="/">home</a>
    <a use:inertia href="/about">about</a>
    <a use:inertia href="/contact">contact</a>
  </header>
  
  <article>
    <slot />
  </article>
</main>