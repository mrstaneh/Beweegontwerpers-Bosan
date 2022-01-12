<script>
    import InhoudItem from "$lib/InhoudItem.svelte";
    import TimelineSprint1 from "$lib/TimelineSprint1.svelte";
</script>
  
<svelte:head>
<title>Sprint 1</title>
</svelte:head>

<main>
    <div class="left-bar" />
    <div class="content">
        <div class="item item-1">
            <img class="item-img" src="/images/personas/lucajansen.png" alt="Luca Jansen"/>
            <div class="item-text">
                <p class="item-name">Luca Jansen</p>
                <p class="item-dsc">"Vrienden kun je ook online maken!"</p>
            </div>
            <button class="item-btn">Meer informatie</button>
        </div>
        <div class="item item-2">
            <img class="item-img" src="/images/personas/mariecdriesen.png" alt="Mariec Driesen"/>
            <div class="item-text">
                <p class="item-name">Mariec Driesen</p>
                <p class="item-dsc">"Een dag niet gezongen is een dag niet geleefd."</p>
            </div>
            <button class="item-btn">Meer informatie</button>
        </div>
        <div class="item item-3">
            <img class="item-img" src="/images/personas/casperdehaan.png" alt="Casper de Haan"/>
            <div class="item-text">
                <p class="item-name">Casper de Haan</p>
                <p class="item-dsc">"Je moet schieten, anders kun je niet scoren."</p>
            </div>
            <button class="item-btn">Meer informatie</button>
        </div>
        <div class="item item-4">
            <img class="item-img" src="/images/personas/rafaelmanikmas.png" alt="Rafaël Manik Mas"/>
            <div class="item-text">
                <p class="item-name">Rafaël Manik Mas</p>
                <p class="item-dsc">"Je bent moediger dan je gelooft, sterker dan je eruit ziet en slimmer dan je denkt. -Winnie de Poeh"</p>
            </div>
            <button class="item-btn">Meer informatie</button>
        </div>
        <div class="item item-5">
            <img class="item-img" src="/images/personas/jorisreiners.png" alt="Joris Reiners"/>
            <div class="item-text">
                <p class="item-name">Joris Reiners</p>
                <p class="item-dsc" style="font-size: 15px;">"Het mooiste aan docent zijn op een basisschool is dat ik mag werken met een bak aan jong talent."</p>
            </div>
            <button class="item-btn">Meer informatie</button>
        </div>
        <div class="item item-6">
            <img class="item-img" src="/images/personas/nickydevries.png" alt="Nicky de Vries"/>
            <div class="item-text">
                <p class="item-name">Nicky de Vries</p>
                <p class="item-dsc">"Geef nooit op! Zet door, ook als het moeilijk wordt."</p>
            </div>
            <button class="item-btn">Meer informatie</button>
        </div>
        <div class="item item-5">
            <img class="item-img" src="/images/personas/marcdegroot.png" alt="Marc de Groot"/>
            <div class="item-text">
                <p class="item-name">Marc de Groot</p>
                <p class="item-dsc">"De kinderen moeten zichzelf ontwikkelen en uitzoeken wat hun het leukste vinden om te doen."</p>
            </div>
            <button class="item-btn">Meer informatie</button>
        </div>
        <div class="item item-6">
            <img class="item-img" src="/images/personas/amyankers.png" alt="Amy Ankers"/>
            <div class="item-text">
                <p class="item-name">Amy Ankers</p>
                <p class="item-dsc" style="font-size: 14px;">"Ik vind het belangrijk dat ik de kinderen enthousiast kan maken met de nieuwe kennis die ze van mij kunnen leren."</p>
            </div>
            <button class="item-btn">Meer informatie</button>
        </div>
    </div>
    <div class="right-bar" />
</main>

<style>
    main {
        display: grid;
        grid-template-columns: 400px 1120px 400px;
        grid-auto-flow: column;
    }

    .content{
        display: grid;
        grid-template-rows: calc(50vh - 32px) calc(50vh - 32px);
        grid-template-columns: 25% 25% 25% 25%;
    }

    .item{
        margin: 8px;
        text-align: left;
        background-color: #ccd7ff;
        border-radius: 8px;
        cursor: pointer;
    }

    .item:hover{
        border: 1px solid white;
    }

    .item-img{
        width: 100%;
        height: 256px;
        object-fit: fill;
        border-top-left-radius: 8px;
        border-top-right-radius: 8px;
    }

    .item-name{
        margin-top: 0px;
        margin-bottom: 0px;
        font-weight: bold;
        margin-left: 6px;
        font-size: 20px;
    }

    .item-dsc{
        margin-top: 2px;
        margin-left: 6px;
    }

    .item-text{
        padding-left: 10px;
        padding-right: 10px;
        padding-top: 10px;
        margin-top: -4px;
        height: 119px;
    }

    .item-btn{
        width: 100%;
        background-color: #004B8E;
        color: rgb(225, 225, 225);
        height: 32px;
        font-size: 16px;
        border: none;
        outline: none;
        border-bottom-left-radius: 8px;
        border-bottom-right-radius: 8px;
    }
</style>