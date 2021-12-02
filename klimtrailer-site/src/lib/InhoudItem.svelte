<script>
    export let paginaNaam = undefined;
    export let scrollToId = undefined;

    function gotoPageSection(){
        try{
            document.getElementById(scrollToId).scrollIntoView({
                behavior: 'smooth'
            });
        }catch{
            console.error('Could not scroll to ID ' + scrollToId);
        }
    }
</script>

<div class="inhoud-item" on:click={gotoPageSection}>
    <i class="icon fa-solid fa-chevron-right"></i><h2>{paginaNaam}</h2>
</div>

<style>
    .inhoud-item:hover{
        cursor: pointer;
    }

    .inhoud-item:hover .icon{
        color: #4491DA;
        transition-duration: 100ms;
    }

    .inhoud-item:hover h2{
        color: #4491DA;
        transition-duration: 100ms;
    }

    .icon{
        display: inline;
        margin-right: 16px;
        font-size: 24px;
    }

    h2{
        display: inline;
        font-size: 24px;
    }

    .inhoud-item{
        margin-bottom: 12px;
    }
</style>