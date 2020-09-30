<script context="module">
  import { writable } from 'svelte/store'
  export const title = writable(null)
</script>

<script>
  import { inertia, page } from '@inertiajs/inertia-svelte'
  import { route } from '@/utils'
</script>
  
<svelte:head>
  <title>{title ? `${title} - Awesome App` : 'Awesome App'}</title> 
 
</svelte:head>
  
<main>
  <header class='capitalize'>
    <a use:inertia href="/">home</a>
    <a use:inertia href="/about">about</a>
    <a use:inertia href="/contact">contact</a>
  </header>
  
  <article>
    <slot />
  </article>
</main>