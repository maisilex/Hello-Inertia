<script context="module">
  import Layout, { title } from '@/Shared/Layout.svelte'

  export const layout = Layout
</script>

<script>
  import { inertia } from '@inertiajs/inertia-svelte'
  $title = 'Welcome'
  export let user
</script>


<h1>Welcome</h1>
<p>Hello {user = 'Alex'}, welcome to your first Inertia app!</p>


