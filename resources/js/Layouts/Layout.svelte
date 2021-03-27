<script context="module">
  import { writable } from 'svelte/store'
  export const title = writable(null)
</script>

<script>
  // import { inertia, page } from '@inertiajs/inertia-svelte'
  // import { route } from '@/Utils'
  // import Dropdown from '@/Shared/Dropdown.svelte'
  // import FlashMessages from '@/Shared/FlashMessages.svelte'
  // import Icon from '@/Shared/Icon.svelte'
  // import Logo from '@/Shared/Logo.svelte'
  // import MainMenu from '@/Shared/MainMenu.svelte'
  import Navbar from '@/Layouts/Navbar.svelte'
</script>

<svelte:head>
  <title>{$title ? `${$title} - Demo App` : 'Demo App'}</title>
</svelte:head>

<Navbar />

<main class="bg-white min-h-screen flex justify-center items-center">
  <slot />
</main>