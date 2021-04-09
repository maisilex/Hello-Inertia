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
  import Navbar from '@/Shared/Navbar.svelte'
</script>

<svelte:head>
   <!-- Primary Meta Tags -->
   <title>{$title ? `${$title} - Demo App` : 'Demo App'}</title>
  

   <meta name="title" content="Example Title">
   <meta name="description" content=" Example description">
     
     <!-- Open Graph / Facebook -->
   <meta property="og:type" content="website">
   <meta property="og:url" content="https://inertia.maisilex.com/">
   <meta property="og:title" content="Example title">
   <meta property="og:description" content="Example description">
   <meta property="og:image" content="">
     
     <!-- Twitter -->
   <meta property="twitter:card" content="summary_large_image">
   <meta property="twitter:url" content="https://inertia.maisilex.com/">
   <meta property="twitter:title" content="Example title">
   <meta property="twitter:description" content="Example description">
   <meta property="twitter:image" content="">
</svelte:head>

<Navbar />

<main class="bg-white min-h-screen flex flex-col justify-center items-center">
  <slot />
</main>