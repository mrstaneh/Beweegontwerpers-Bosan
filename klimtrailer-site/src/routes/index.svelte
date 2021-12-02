<script>
    import InhoudItem from "$lib/InhoudItem.svelte";
import SlideShow from "$lib/SlideShow.svelte";
    import Timeline from "$lib/Timeline.svelte";

    let currentDate = new Date();

    let students = [
        {
            name: 'Britney Janssen',
            email: 'britney.janssen@student.fontys.nl',
            role: 'Notulist'
        },
        {
            name: 'Loes Käller',
            email: 'l.kaller@student.fontys.nl',
            role: 'Contactpersoon'
        },
        {
            name: 'Matthijs de Vries',
            email: 'm.devries@student.fontys.nl',
            role: 'Teamlid'
        },
        {
            name: 'Rick Peters',
            email: 'r.peters-ab@student.fontys.nl',
            role: 'Teamleider'
        },
        {
            name: 'Stan Jaworski',
            email: 's.jaworski@student.fontys.nl',
            role: 'Scrum Master'
        },
        {
            name: 'Wout Ploumen',
            email: 'w.ploumen@student.fontys.nl',
            role: 'Teamlid'
        }
    ]
</script>

<div class="home-image-container">
    <img class="home-image" src="bosan.jpg" alt="">
</div>
<main>
    <div class="left-bar">
        
    </div>
    <div class="content">
        <!--<div class="section start">
            <h1>Portfolio</h1>
        </div>-->
        <div class="voorpagina">
            <h1 style="font-size: 90px; margin-top: 0px; margin-bottom: 0px; color: #F06119;">PORTFOLIO</h1>
            <h2 style="font-size: 50px; margin-top: 100px; color: #F06119;">Bosan B.V.</h2>
        </div>
        <div class="gegevens">
            <h1>Gegevens</h1>

            <div class="gegevens-container">
                <div class="gegevens-column">
                    <p>Studenten</p>
                    {#each students as student}
                        <div class="gegevens-item">
                            <p><b>Naam:</b> {student.name}</p>
                            <p><b>Email:</b> <a href="mailto:{student.email}">{student.email}</a></p>
                            <p><b>Rol:</b> {student.role}</p>
                        </div>
                    {/each}
                </div>
                <div class="gegevens-column">
                    <p>Verslag</p>
                    <div class="gegevens-item">
                        <p><b>Titel:</b> ........</p>
                        <p><b>Versie:</b> 1</p>
                        <p><b>Datum:</b> {currentDate.getDay()}-{currentDate.getMonth()}-{currentDate.getFullYear()}</p>
                    </div>

                    <p style="margin-top: 54px;">Bedrijf</p>
                    <div class="gegevens-item">
                        <p><b>Naam:</b> Bosan B.V.</p>
                        <p><b>Adres:</b> Metaalstraat 21, 7483 PD Haaksbergen</p>
                        <p><b>Telefoonnummer:</b> 053-3035107</p>
                    </div>

                    <p style="margin-top: 54px;">Opdrachtgever</p>
                    <div class="gegevens-item">
                        <p><b>Contactpersoon:</b> Mark Snijder</p>
                        <p><b>E-mail:</b> <a href="mailto:m.snijder@bosan.nl">m.snijder@bosan.nl</a></p>
                        <p><b>Mobiel telefoonnummer:</b> 06-21246905</p>
                    </div>

                    <p style="margin-top: 54px;">Opdrachtgever</p>
                    <div class="gegevens-item">
                        <p><b>Contactpersoon:</b> Melanie van Deursen</p>
                        <p><b>E-mail:</b> <a href="mailto:m.vandeursen@groupe-abeo.com">m.vandeursen@groupe-abeo.com</a></p>
                    </div>
                </div>
            </div>
            <img class="gegevens-image" src="bosan-2.jpg" alt="">
        </div>
        <div class="voorwoord">
            <h1 style="margin-top: 8px;">Voorwoord</h1>
            <p style="color: #4491DA;">In de periode van september 2021 tot en met januari 2022 hebben wij onze opdracht gelopen voor Bosan B.V. 
                – Bosan ontwikkelt en produceert sportinstallaties en sporttoestellen voor bewegingsonderwijs en (top)sport in binnensportaccommodaties.</p>

            <p>Dit verslag is geschreven in het kader van onze minor aan de Fontys Sporthogeschool en in opdracht voor onze stakeholder Bosan.
                Tijdens het semester is er onderzoek gedaan naar een nieuw toestel voor Bosan. Dit toestel zal buiten toepasbaar moeten zijn zodat basisscholen meer ruimte hebben om beweegonderwijs te geven en daardoor de 2 uur per week voor een kind kunnen halen.
                </p>

                <p>In dit verslag beschrijven we het proces van het project. Voor het proces hebben gebruik gemaakt van de design thinking methode.</p>
        </div>
        <div class="section inhoud">
            <h1>Inhoud</h1>
            <InhoudItem paginaNaam="Samenvatting" scrollToId="samenvatting"/>
            <InhoudItem paginaNaam="Woordenlijst" scrollToId="woordenlijst"/>
            <InhoudItem paginaNaam="Inleiding" scrollToId="inleiding"/>
            <InhoudItem paginaNaam="Opdrachtgever" scrollToId="opdrachtgever"/>
            <InhoudItem paginaNaam="Opdracht" scrollToId="opdracht"/>
        </div>
        <div class="section samenvatting" id="samenvatting">
            <h1>Samenvatting</h1>

            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget nisi sit amet est rhoncus tristique. Nam rhoncus lectus non tempor condimentum. Duis efficitur fringilla lacus, a ornare nisl mollis vitae. Sed luctus porttitor congue. Donec efficitur dictum sapien sit amet euismod. Phasellus iaculis ac erat convallis cursus. Donec id ex ut ipsum sagittis rhoncus a eu urna. Fusce dapibus urna eget leo porttitor vestibulum.</p>
            <p>Nulla egestas id tellus ut faucibus. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec posuere nec libero ut pulvinar. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Nullam finibus lacus placerat leo auctor, in hendrerit est dapibus. In finibus lorem lacus, ut vestibulum ipsum venenatis eu. Quisque quis risus ut ligula rutrum tempus non non diam. Nam ac eros dui. Mauris dictum sapien finibus mi vulputate congue. Nam aliquet non felis in dictum. </p>
            <p>Cras vel consectetur dolor. Vestibulum lacinia consectetur tempus. Quisque sit amet accumsan libero. Nam iaculis tempor mauris. Vestibulum eu sodales ipsum. Suspendisse pretium, ante id elementum lacinia, ante nunc rhoncus tellus, non tempor elit nunc id magna. Cras vel convallis nibh. Aenean dapibus ut ante non auctor. Maecenas sed pellentesque ex. Morbi vel efficitur ex, non hendrerit urna.</p>
            <p>Nulla egestas id tellus ut faucibus. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec posuere nec libero ut pulvinar. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Nullam finibus lacus placerat leo auctor, in hendrerit est dapibus. In finibus lorem lacus, ut vestibulum ipsum venenatis eu. Quisque quis risus ut ligula rutrum tempus non non diam. Nam ac eros dui. Mauris dictum sapien finibus mi vulputate congue. Nam aliquet non felis in dictum. </p>

            <SlideShow/>
        </div>
        <div class="section woordenlijst" id="woordenlijst">
            <h1>Woordenlijst</h1>
        </div>
        <div class="section inleiding" id="inleiding">
            <h1>Inleiding</h1>

            <p style="color: #F06119; display: inline;">“2 UUR GYMLES VERPLICHT PER WEEK VANAF 2023 VOOR ALLE BASISSCHOLEN MET  EEN BEVOEGDE LEERKRACHT”</p>
            <p style="display: inline;"> (Ministerie van Volksgezondheid, 2021)</p>

            <p>Scholen die meedoen kunnen een beweegvignet krijgen door kinderen meer te laten bewegen. Welke school wilt dit nou niet? </p>
            <p>Dit sluit aan bij het programma van Gezonde school en Gezonder kinderopvang. Tevens zal er gezorgd worden voor buitenspeelplekken en sportaanbod in de wijk. Bij de inrichting van wijken moeten gemeenten meer beweegplekken creëren. Zodat buitenspelen weer aantrekkelijk wordt voor kinderen. Bijvoorbeeld sportactiviteiten organiseren op de aangrenzende velden, met hulp van een lokale sportcoach. Alleen of dit de juiste aanpak is valt over te discussiëren  </p>
            <p style="color: #F06119; display: inline;">“ALS JE BEWEGING VAN JONGS AF AAN STIMULEERT, ZULLEN ZE OP LATERE LEEFTIJD OOK MEER BLIJVEN BEWEGEN EN SPORTEN.”</p>
            <p> Nederlandse kinderen speelden in 2019 gemiddeld 8,4 uur per week buiten. Dat gemiddelde wordt vooral bepaald door de 28 procent die nog méér buiten speelt. Toch zit bijna 60 procent onder dit gemiddelde en speelt zelfs 15 procent nooit buiten. <a href="https://jantjebeton.nl/uploads/downloads/onderzoek-buitenspelen-2019-5cffc1bd70afd.pdf" target="_blank">Blijkt uit onderzoek van Jantje Beton</a>
        </div>
        <div class="section opdrachtgever" id="opdrachtgever">
            <h1>Opdrachtopgever</h1>  
            <p style="color: #4491DA;">Wie regelmatig sport en beweegt leeft gezonder. Bosan staat voor een gezonde wereld en ontwikkelt en produceert hiervoor innovatieve, doordachte, kwalitatief hoogwaardige sporttoestellen en -installaties</p>  
            <p>Bosan is opgericht in 1973 door oud topturner Gerrit ten Bos in zijn garage met het verbeteren van landingsmatten. Vandaag de dag is Bosan een bloeiende onderneming en vestigt het zich in Haaksbergen en Melle. Bosan richt zich op het ontwikkelen en produceren van sporttoestellen en -installaties. Verder richten ze ook complete sportaccommodaties in, met het accent op bewegingsonderwijs en (top)sport. De producten zijn te vinden in ruim 1800 sportaccommodaties in Nederland en daarbuiten. Ze doen alles zelf, van ontwerp tot fabricage tot plaatsen tot transport</p>
            <p>Bosan is een zelfbewuste onderneming; ze weten wat ze kunnen. Ze zijn trots op hun producten en diensten en op zijn vermogen tot vernieuwen en verbeteren. Steeds brengen ze innovatieve concepten en productontwikkelingen. De elektrisch verrolbare werkbalk, de zwaaipuntverlager, de inzinkbare rekstokzuil, de korfbal/springstandaard met dempingsysteem, de Piré springkasten, de basketbalinstallatie met ledverlichting, het elektrische klimrek en de turnmatten zijn hiervan enkele voorbeelden. Deze installaties zijn niet meer weg te denken uit het moderne bewegingsonderwijs en in binnensportaccommodaties. Voor deze installaties maken ze vrijwel alleen gebruik van duurzame materialen en kwalitatief sterk materiaal.</p> 
        </div> 
    </div>
    <div class="right-bar">
        <div class="voorpagina"></div>
        <Timeline/>
    </div>
</main>

<style>
    main{
        display: grid;
        grid-template-columns: 300px 960px 660px;
        grid-auto-flow: column;
    }

    .section{
        border-top: 1px solid black;
        text-align: left;
    }

    .voorpagina{
        height: 100vh;
        text-align: center;
    }

    .gegevens-container{
        display: grid;
        grid-template-columns: 55% 45%;
        grid-auto-flow: column;
    }

    .gegevens-column p{
        margin-top: 0px; 
        color: #F06119; 
        font-weight: bold;
        margin-bottom: 4px;
    }

    .gegevens-item{
        margin-bottom: 16px;
    }

    .gegevens-item p{
        color: black;
        font-weight: normal;
        margin-top: 0px;
        margin-bottom: 0px;
    }

    .gegevens-image{
        width: 100%;
    }

    .home-image{
        justify-content: start;
        position: absolute;
        left: 0;
        width: 100%;
        height: 100vh;
        object-fit: cover;
        z-index: -1;
        filter: sepia(300%) saturate(50%) brightness(70%) hue-rotate(180deg);
    }
</style>