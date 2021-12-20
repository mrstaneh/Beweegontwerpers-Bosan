<script>
    import Nav from "$lib/Nav.svelte";
    import { page } from '$app/stores';
</script>

<Nav pagePath={$page.path}/>
<slot />