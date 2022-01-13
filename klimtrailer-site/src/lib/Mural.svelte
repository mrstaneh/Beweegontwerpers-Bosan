<script>
    export let title = undefined;
    export let src = undefined;

    let enlarged = false;
    let bgColor = 'rgb(101, 214, 116)';
    let bgHoverColor = 'rgb(121, 234, 136)';

    function onEnlargeClick(){
        enlarged = !enlarged;

        document.getElementById(`mural-${title}`).src = document.getElementById(`mural-${title}`).src;
    }
</script>

<div class="mural-container" style="{enlarged == true ? 'position: fixed; left: 5vw; top: 8vh; width: 90vw; height: 84vh; z-index: 999;' : ''}">
    <div class="mural-bar">
        <p>{title} Mural</p>
        <div class="mural-bar-right">
            <p style="margin-right: 8px;">Dit is een interactief component</p>
            <button on:click={onEnlargeClick} style="{enlarged == true ? '--bg-color: rgb(214, 101, 101); --bg-hover-color: rgb(234, 121, 121);' : '--bg-color: rgb(101, 214, 116); --bg-hover-color: rgb(121, 234, 136);'}">{enlarged == true ? 'Verklein' : 'Vergroot'}</button>
        </div>
    </div>
    <div class="mural-iframe">
        <iframe title="{title}" src='{src}'
        width='99.8%'
        id="mural-{title}"
        height='{enlarged == true ? '90vw' : '480px'}'
        style='min-width: 640px; {enlarged == true ? 'min-height: 84vh;' : 'min-height: 480px;'} background-color: #efefef; border: 1px solid #c0c0c0'
        sandbox='allow-same-origin allow-scripts allow-modals allow-popups allow-popups-to-escape-sandbox'>
        </iframe>
    </div>
</div>

<style>

    p{
        display: inline;
        margin-bottom: 0px;
        margin-top: 0px;
        margin-left: 8px;
    }

    .mural-bar{
        height: 24px;
    }

    .mural-bar-right{
        height: 24px;
        float: right;
    }

    .mural-bar-right button{
        position: relative;
        height: 24px;
        top: -1px;
        border-top-right-radius: 8px;
        border: none;
        border-left: 1px solid #c0c0c0;
        outline: none;
        background-color: var(--bg-color);
    }

    .mural-bar-right button:hover{
        background-color: var(--bg-hover-color);
        cursor: pointer;
    }

    .mural-bar{
        border-top-left-radius: 8px;
        border-top-right-radius: 8px;
        border-left: 1px solid #c0c0c0;
        border-right: 1px solid #c0c0c0;
        border-top: 1px solid #c0c0c0;
        background-color: #e7ecff;
    }
</style>