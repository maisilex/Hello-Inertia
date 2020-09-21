<script context="module">
  import Layout from '@/Shared/Layout.svelte'
  export const layout = Layout
</script>

<script>
  export let user
</script>



<h1>Contact</h1>
<p>Hello {user = 'Alex'}, welcome to your first Inertia app!</p>
