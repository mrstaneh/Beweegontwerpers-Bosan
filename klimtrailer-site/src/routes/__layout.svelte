<script>
    import Nav from "$lib/Nav.svelte";
    import { page } from '$app/stores';
    import PageTransitions from "$lib/PageTransitions.svelte";
</script>

<Nav pagePath={$page.path}/>
<PageTransitions refresh={$page.path}>
    <slot />
</PageTransitions>