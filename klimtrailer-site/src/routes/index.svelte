<script>
    import Timeline from "$lib/Timeline.svelte";
</script>

<div class="home-image">
    <p>Mini Boulder</p>
</div>

<main>
    <div class="left-bar">
        
    </div>
    <div class="content">
        <!--<div class="section start">
            <h1>Portfolio</h1>
        </div>-->
        <div class="voorwoord">
            <h1>Voorwoord</h1>
            <p style="color: #4491DA;">In de periode van september 2021 tot en met januari 2022 hebben wij onze opdracht gelopen voor Bosan B.V. 
                – Bosan ontwikkelt en produceert sportinstallaties en sporttoestellen voor bewegingsonderwijs en (top)sport in binnensportaccommodaties.</p>

            <p>Dit verslag is geschreven in het kader van onze minor aan de Fontys Sporthogeschool en in opdracht voor onze stakeholder Bosan.
                Tijdens het semester is er onderzoek gedaan naar een nieuw toestel voor Bosan. Dit toestel zal buiten toepasbaar moeten zijn zodat basisscholen meer ruimte hebben om beweegonderwijs te geven en daardoor de 2 uur per weer voor een kind kunnen halen.
                </p>

                <p>In dit verslag beschrijven we het proces van het project. Voor het proces hebben gebruik gemaakt van de design thinking methode.</p>
        </div>
        <div class="section samenvatting">
            <h1>Samenvatting</h1>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget nisi sit amet est rhoncus tristique. Nam rhoncus lectus non tempor condimentum. Duis efficitur fringilla lacus, a ornare nisl mollis vitae. Sed luctus porttitor congue. Donec efficitur dictum sapien sit amet euismod. Phasellus iaculis ac erat convallis cursus. Donec id ex ut ipsum sagittis rhoncus a eu urna. Fusce dapibus urna eget leo porttitor vestibulum.</p>
            <p>Nulla egestas id tellus ut faucibus. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec posuere nec libero ut pulvinar. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Nullam finibus lacus placerat leo auctor, in hendrerit est dapibus. In finibus lorem lacus, ut vestibulum ipsum venenatis eu. Quisque quis risus ut ligula rutrum tempus non non diam. Nam ac eros dui. Mauris dictum sapien finibus mi vulputate congue. Nam aliquet non felis in dictum. </p>
            <p>Cras vel consectetur dolor. Vestibulum lacinia consectetur tempus. Quisque sit amet accumsan libero. Nam iaculis tempor mauris. Vestibulum eu sodales ipsum. Suspendisse pretium, ante id elementum lacinia, ante nunc rhoncus tellus, non tempor elit nunc id magna. Cras vel convallis nibh. Aenean dapibus ut ante non auctor. Maecenas sed pellentesque ex. Morbi vel efficitur ex, non hendrerit urna.</p>
            <p>Nulla egestas id tellus ut faucibus. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec posuere nec libero ut pulvinar. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Nullam finibus lacus placerat leo auctor, in hendrerit est dapibus. In finibus lorem lacus, ut vestibulum ipsum venenatis eu. Quisque quis risus ut ligula rutrum tempus non non diam. Nam ac eros dui. Mauris dictum sapien finibus mi vulputate congue. Nam aliquet non felis in dictum. </p>
        </div>
    </div>
    <div class="right-bar">
        <Timeline/>
    </div>
</main>

<style>
    main{
        display: grid;
        grid-template-columns: 480px 960px 480px;
        grid-auto-flow: column;
    }

    .section{
        border-top: 1px solid black;
        text-align: left;
    }

    /*.backdrop{
        justify-content: start;
        position: absolute;
        left: 0;
        width: 100vw;
        height: 100vh;
        z-index: -1;
        filter: sepia(10%) saturate(100%) brightness(70%) hue-rotate(10deg);
    }*/
</style>