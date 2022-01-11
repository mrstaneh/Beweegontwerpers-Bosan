<script>
    import { fade } from 'svelte/transition';
    export let refresh = '';
</script>
  
{#key refresh}
    <div in:fade={{ delay: 50, duration: 100 }}>
        <slot/>
    </div>
{/key}