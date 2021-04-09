<script context="module">
  import Layout, { title, metaTitle } from '@/Shared/Layout.svelte'
  export const layout = Layout
</script>
  
<script>
  // TODO: 
  // import { inertia, page } from '@inertiajs/inertia-svelte'
  // import { route } from '@/Utils'
  // import Icon from '@/Shared/Icon.svelte'
  // import Pagination from '@/Shared/Pagination.svelte'
  // import SearchFilter from '@/Shared/SearchFilter.svelte'
  // export let contacts = []
  $title = 'Welcome'
  $metaTitle = 'Ghdjsjhdsgfjsdgfjhsdgfjhsdgjfhsg'
  // let filters = {
  //   trashed: $page.props.filters.trashed,
  // }
  export let laravelVersion
  export let phpVersion
</script>
  
<h1 class="text-6xl sm:text-8xl">Hey there!!!</h1>

<div class="mt-10 text-4xl sm:text-6xl text-gray-500">
    Laravel v{ laravelVersion } (PHP v{ phpVersion }) 
</div>
  