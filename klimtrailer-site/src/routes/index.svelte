<script>
  import TitleScreen from "$lib/TitleScreen.svelte";
</script>

<svelte:head>
  <title>Bosan Portfolio</title>
</svelte:head>

<svelte:window />

<div id="titleScreen">
  <TitleScreen />
</div>

<main>
  <div class="content">
    <!--<div class="section start">
            <h1>Portfolio</h1>
        </div>-->

    <div class="voorwoord">
      <h1 style="margin-top: 8px;">Voorwoord</h1>
      <p style="color: #4491DA;">
        In de periode van september 2021 tot en met januari 2022 hebben wij onze opdracht gelopen voor Bosan B.V. – Bosan ontwikkelt en produceert sportinstallaties en sporttoestellen voor bewegingsonderwijs en (top)sport in binnensportaccommodaties.
      </p>

      <p>
        Dit verslag is geschreven in het kader van onze minor aan de Fontys Sporthogeschool en in opdracht voor onze stakeholder Bosan.
        Tijdens het semester is er onderzoek gedaan naar een nieuw toestel voor Bosan. Dit toestel zal buiten toepasbaar moeten zijn zodat basisscholen meer ruimte hebben om beweegonderwijs te geven en daardoor de 2 uur per weer voor een kind kunnen halen.

      </p>

      <p>
        In dit verslag beschrijven we het proces van het project. Voor het proces hebben gebruik gemaakt van de design thinking methode.
      </p>
    </div>
    <!-- <div class="section inhoud" id="inhoud">
      <h1>Inhoud</h1>
      <InhoudItem paginaNaam="Samenvatting" scrollToId="samenvatting" />
      <InhoudItem paginaNaam="Woordenlijst" scrollToId="woordenlijst" />
      <InhoudItem paginaNaam="Inleiding" scrollToId="inleiding" />
      <InhoudItem paginaNaam="Opdrachtgever" scrollToId="opdrachtgever" />
      <InhoudItem paginaNaam="Opdracht" scrollToId="opdracht" />
      <InhoudItem paginaNaam="Brainstorm" scrollToId="brainstorm" />
      <InhoudItem paginaNaam="Frames" scrollToId="frames" />
      <InhoudItem paginaNaam="Prototyping" scrollToId="prototyping" />
      <InhoudItem paginaNaam="Proces" scrollToId="proces" />
    </div> -->
    <div class="section samenvatting" id="samenvatting">
      <h1>Samenvatting</h1>

      <p>
        Hoeveel beweging heeft een kind gemiddeld nodig? Volgens de beweegrichtlijnen hebben basisschoolkinderen minimaal 1 uur matige, intensieve beweging nodig om gezond te blijven. Voldoende beweging is goed voor de gezondheid en de ontwikkeling van het kind, dit zorgt tevens voor een verhoging in het zelfvertrouwen en de sociale vaardigheden. 
      </p>
      <p>
        Bosan wil een nieuwe ontwikkeling realiseren om met innovatieve materialen de beweging bij kinderen te stimuleren in het beweegonderwijs. Opdrachtgever Bosan kwam vervolgens met de hoofdvraag: “Op welke wijze kunnen we met innovatieve materialen beweegomgevingen inrichten zodat ze aansluiten bij de ontwikkeling in het bewegingsonderwijs?”. Uit onderzoek blijkt: “Vanaf 2023 geldt een nieuwe regel, kinderen op de basisschool moeten verplicht minimaal 2 uur per week gymles krijgen.” Uit onderzoek is helder geworden dat niet iedere basisschool voldoende capaciteit heeft  , daarom is de stap ondernomen om de focus te leggen op buiten gymmen. De design thinking methode is toegepast tijdens het proces, er is gebruik gemaakt van: brainstormsessies, iteratief en incrementeel werken, vormgeven van persona’s, korte testen doen en diverse interviews houden met experts. De Boulder Mini is op diverse momenten geoptimaliseerd, zo is er bijvoorbeeld gekeken naar de wetgeving rondom verplichte valmatten en het multifunctioneel inzetten van prototypes. Daarnaast zijn ook de praktische eisen in acht genomen, zoals de hanteerbaarheid van het product. Uiteindelijk is de Boulder Mini ontstaan met diverse demonteerbare wanden. 
      </p>
      <p>
        Er is gekozen voor een aanhanger naar aanleiding van het onderzoek naar de regelgeving. Het is mogelijk om naast het aanschaffen van het product een leasecontract en een onderhoudsplan aan te schaffen. Voordat het productproces afgerond is zijn er ter voor de volledige validatie meerdere interviews gehouden met experts. De experts waren enthousiast over het product. Het product bestaat uit een verplaatsbare klimwand. De klimwanden zijn verstelbaar in diverse kantelhoeken en klimmethodes. Een quote vanuit Stefan van Veen (master in Sport- en Beweeginnovatie):
      </p>
      <p style="font-size: 18px; color: #F06119;">
        “Het product heeft zeker meerwaarde en kent een multifunctionele werkvorm toe.”
      </p>
    </div>
    <div class="section samenvatting-interviews" id="samenvatting-interviews">
      <h1>Samenvatting Interviews</h1>
      <p>Om diepgang te creëren in onze persona’s en om ons te kunnen verplaatsen in de doelgroep, hebben we verschillende interviews gedaan.</p>
      <p>Esther (basisschool docent geweest) en Tess (gymdocent) geven beide aan dat groepsleerkrachten met de bevoegdheid om gymles te geven vaak terugvallen op vormen die ze kennen. Het belang van goed beweegonderwijs wordt minder ingeschat. </p>
      <p>Alle geïnterviewden geven aan dat een gymtoestel genoeg variatie moet bieden voor de kinderen. Aldus Anoek (onderzoeker beweegonderwijs): “Het is handig als een toestel op meerdere manieren gebruikt kan worden." En “De kinderen moeten enthousiast worden bij het zien van het toestel, omdat ze allemaal op hun eigen manier uitgedaagd worden.” Naast de variatie moet het toestel ook veilig genoeg zijn. Esther: “Spellen moeten zo veilig mogelijk zijn.” </p>
      <p>Daarnaast is het belangrijk dat het toestel tegen een stootje kan, geven Esther, Anoek en Marc (klimdocent) aan. Het gymtoestel moet dus ‘hufterproof’ zijn en moet ook beschermd worden tegen oneigenlijk gebruik wanneer het zich op het speelplein bevindt. </p>
      <p>Er wordt hedendaags nog maar weinig gebruik gemaakt van het buiten gymmen. Aldus Anoek “Er zijn bijna geen scholen die doen aan buiten gymmen.” Echter is hier wel animo voor, aldus Tess “Ik zou wel vaker buiten willen gymmen, zodra dit toegankelijker is.” </p>
      <p>Voor de volledige interviews zie de <a href="/bijlagen#2" target="_blank">bijlage.</a></p>
    </div>
    <div class="section inleiding" id="inleiding">
      <h1>Inleiding</h1>

      <p style="color: #F06119; display: inline;">
        “2 uur gymles verplicht per week vanaf 2023 voor alle basisscholen met
        een bevoegde leerkracht”
      </p>
      <p style="display: inline;">(Ministerie van Volksgezondheid, 2021) [<a target="_blank" href="bronvermelding/#6">6</a>]</p>

      <p>
        Scholen die meedoen kunnen een beweegvignet krijgen door kinderen meer
        te laten bewegen. Welke school wilt dit nou niet?
      </p>
      <p>
        Dit sluit aan bij het programma van Gezonde school en Gezonder
        kinderopvang. Tevens zal er gezorgd worden voor buitenspeelplekken en
        sportaanbod in de wijk. Bij de inrichting van wijken moeten gemeenten
        meer beweegplekken creëren. Zodat buitenspelen weer aantrekkelijk wordt
        voor kinderen. Bijvoorbeeld sportactiviteiten organiseren op de
        aangrenzende velden, met hulp van een lokale sportcoach. Alleen of dit
        de juiste aanpak is valt over te discussiëren
      </p>
      <p style="color: #F06119; display: inline;">
        “Als je beweging van jongs af aan stimuleert, zullen ze op latere
        leeftijd ook meer blijven bewegen en sporten.”
      </p>
      <p>
        Nederlandse kinderen speelden in 2019 gemiddeld 8,4 uur per week buiten.
        Dat gemiddelde wordt vooral bepaald door de 28 procent die nog méér
        buiten speelt. Toch zit bijna 60 procent onder dit gemiddelde en speelt
        zelfs 15 procent nooit buiten. [<a target="_blank" href="bronvermelding/#17">17</a>] 
      </p>
    </div>
    <div class="section opdrachtgever" id="opdrachtgever">
      <h1>Opdrachtopgever</h1>
      <p style="color: #4491DA;">
        Wie regelmatig sport en beweegt leeft gezonder. Bosan staat voor een gezonde wereld en ontwikkelt en produceert hiervoor innovatieve, doordachte, kwalitatief hoogwaardige sporttoestellen en -installaties.
      </p>
      <p>
        Bosan is opgericht in 1973 door oud topturner Gerrit ten Bos in zijn garage met het verbeteren van landingsmatten. Vandaag de dag is Bosan een bloeiende onderneming  en vestigt het zich in Haaksbergen en Melle. Bosan richt zich op het ontwikkelen en produceren van sporttoestellen en -installaties. Verder richten ze ook complete sportaccommodaties in, met het accent op bewegingsonderwijs en (top)sport. De producten zijn te vinden in ruim 1800 sportaccommodaties in Nederland en daarbuiten. Ze doen alles zelf, van ontwerp tot fabricage tot plaatsen tot transport.
      </p>
      <p>
        Bosan is een zelfbewuste onderneming; ze weten wat ze kunnen. Ze zijn trots op hun producten en diensten en op zijn vermogen tot vernieuwen en verbeteren. Steeds brengen ze innovatieve concepten en productontwikkelingen. De elektrisch verrolbare werkbalk, de zwaaipuntverlager, de inzinkbare rekstokzuil, de korfbal/springstandaard met dempingsysteem, de Piré springkasten, de basketbalinstallatie met ledverlichting, het elektrische klimrek en de turnmatten zijn hiervan enkele voorbeelden. Deze installaties zijn niet meer weg te denken uit het moderne bewegingsonderwijs en in binnensportaccommodaties. Voor deze installaties maken ze vrijwel alleen gebruik van duurzame materialen en kwalitatief sterk materiaal.
      </p>
      <p>De meest recente innovatie is de elektrische wandtrampoline:</p>
      <img class="opdrachtgever-image" src="images/wandtrampoline.jpg" alt="" />
      <p>
        De passie van Bosan is dat het met innovatieve, doordachte, kwalitatief hoogwaardige sporttoestellen en –installaties, zowel voor de (top)sport als het bewegingsonderwijs, laat Bosan mensen bewegen; jong en oud, valide en minder valide, geoefend en ongeoefend. Het project is opgezet door Mark Snijder (Regio Manager Zuid NL & België) en Melanie van Deursen (Product manager bewegingsonderwijs).
      </p>
    </div>
    <div class="section opdracht" id="opdracht">
      <h1>Opdracht</h1>

      <p style="color: #4491DA;">
        Voor wie maken wij deze opdracht? Wat houdt de opdracht in? Wat zou er bereikt moeten worden?
      </p>

      <p style="color: #F06119; display: inline;">Verwaching vanuit Bosan</p>
      <p class="pheader">
        Vanuit Bosan hebben wij de volgende vraag gekregen: “Op welke wijze kunnen we met innovatieve materialen beweegomgevingen inrichten zodat ze aansluiten bij de ontwikkeling in het bewegingsonderwijs?”. 
      </p>
      <p>
        Bosan verwacht van ons dat we een product ontwikkelen dat ingezet kan worden in het bewegingsonderwijs. Dit kan gaan over een nieuw sportattribuut, een doorontwikkeling op een sportattribuut, een uitbreiding op een sportattribuut of zoiets geks als een digitale muur. Er zou dus van alles bedacht kunnen worden op de opdracht.
      </p>
      <p style="color: #F06119; display: inline;">Onze focus</p>
      <p class="pheader">
        We hebben zelf gekozen om onze focus te leggen op een toestel voor het primair onderwijs dat buiten gebruikt kan worden. Hier hebben wij voor gekozen omdat het primair onderwijs over iets meer dan 2 jaar minimaal 2 uur gym per kind gegeven zou moeten worden 
        (CIOS, 2020)[<a target="_blank" href="bronvermelding/#5">5</a>]. Dit duurt dan wel nog 2 jaar voordat deze wet van kracht gaat. Dit komt doordat de scholen aangeven dat er te weinig gymleraren, sporthallen of sportvelden ter beschikking hebben 
        (CIOS, 2020)[<a target="_blank" href="bronvermelding/#5">5</a>]. 
      </p>
      <p style="color: #F06119; display: inline;">Onze stappen</p>
      <p class="pheader">
        In samenwerking met de stakeholder zijn wij gaan kijken of het vraagstuk zorgt voor voldoende uitdaging. Door in gesprek te gaan met Bosan, is er duidelijk geworden dat zij ook kansen zien in het maken van een buiten toestel. Zoals wij ook al onderzocht hadden zal er binnenort namelijk 2 uur gym gegeven moeten worden, dit zal alleen niet mogelijk zijn omdat de scholen te weinig ruimte hebben of te weinig leraren hebben. Dit zijn goede redenen om te focussen op gymles buiten. 
      </p>
      <p style="color: #F06119; display: inline;">Onze team</p>
      <p class="pheader">
        Het team bestaat uit een multidisciplinaire groep. Zo heeft ieder zijn specialiteiten in de opleiding. Dit is erg uiteenlopend van ICT tot Mechatronica tot Communicatie tot aan Technische bedrijfskunde. Kortom veel diverse opleidingen. Dit kan juist als een voordeel werken. Iedere persoon heeft weer net een andere kijk op een probleem. 
      </p>
      <p>
        Vervolgens is er door ondersteuning van de lessen en het boek “Design thinking” van Guido Stompff. een basis behandeld. 
      </p>
      <img class="opdracht-image" src="images/designthinking.png" alt="" />
      <p>
        Voorafgaand aan dit project is er een volledige designsprint cyclus doorlopen met een andere opdracht. Op deze manier is er dus al eens kennis gemaakt met de cyclus van designthinking. 
      </p>
    </div>
    <a style="margin-bottom: 20px;" href="proces" class="button">Ga naar de volgende pagina</a>
  </div>
</main>

<style>
  main{
    display: flex;
    align-items: center;
    justify-content: center;
  }

  @media(min-width: 1300px){
    .content{
      width: 50%;
    }
  }

  @media(max-width: 1299px){
    .content{
      width: 75%;
    }
  }

  @media(max-width: 750px){
    .content{
      width: 95%;
    }
  }

  .voorwoord {
    text-align: justify;
  }

  .opdracht-image {
    width: 50%;
  }

  .pheader{
    margin-top: 0px;
  }

  #top-button {
    cursor: pointer;
    position: fixed;
    bottom: 20px;
    right: 0px;
    z-index: 1;
    border: none;
    outline: none;
    background-color: #a5a4a4;
    color: #a5a4a4;
    padding: 15px;
    padding-right: 15px;
    border-top-left-radius: 8px;
    border-bottom-left-radius: 8px;
    -webkit-tap-highlight-color: transparent;
  }

  #top-button:hover {
    background-color: #808080;
    transition-duration: 100ms;
  }

  .fa-angles-up {
    font-size: 24px;
    color: #ff9f55;
  }
</style>
