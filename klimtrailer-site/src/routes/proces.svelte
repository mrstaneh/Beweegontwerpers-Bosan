<script>
  import Mural from "$lib/Mural.svelte";
  import TimelineSprint1 from "$lib/TimelineSprint1.svelte";
</script>

<svelte:head>
  <title>Proces</title>
</svelte:head>

<main>
  <div class="left-bar" />
  <div class="content">
    <h1>Proces</h1>
    <div class="section destep/muurkrant" id="destep">
      <h1>DESTEP-Analyse / Muurkrant</h1>
      <p>
        DESTEP is een afkorting en staat voor demografische, economische,
        sociaal/culturele, technologische, ecologische en politiek/juridische
        factoren.
      </p>
      <p>
        Binnen deze sprint zijn we het probleem uiteen gaan zetten doormiddel
        van een DESTEP, die we later op een muurkrant (zie hieronder) gepresenteerd hebben aan onze stakeholder.
      </p>
      <Mural title="Muurkrant" src="https://app.mural.co/embed/80134860-96ce-411d-99e3-084e2abe5c9e"/>
      <p>
        Uit deze muurkrant hebben we een aantal keuzes gemaakt die tot ons
        eerste vraagstuk leiden: “Hoe kunnen we er voor zorgen dat alle <b
          >basisschoolkinderen</b
        >
        minimaal <b>2 uur</b> per week <b>gymles</b> krijgen doormiddel van een
        <b>nieuw toestel</b>
        dat <b>buiten</b> toepasbaar is?"
      </p>
      <p>
        Nu blijven natuurlijk de volgende vragen nog over: Waarom is er gekozen
        voor basisschool leerlingen? Waarom 2 uur per dag? En waarom moet het
        buiten toepasbaar zijn?
      </p>
      <p style="color: #F06119; display: inline;">Onderzoeksresultaten</p>
      <p>
        Als eerst zullen we kijken waarom er 2 uur per dag gym plaatst moet
        vinden. “Scholen in het primair onderwijs worden verplicht om minimaal
        twee uur gym per week te verzorgen. Dat is het resultaat van een
        voorstel van Kamerleden Rudmer Heerema (VVD) en Michiel van Nispen (SP),
        wat door een meerderheid van de Tweede Kamer werd aangenomen. De scholen
        kunnen rekenen op een overgangsperiode van drie jaar om te voldoen aan
        de verplichte twee uur gym per schoolweek.”[<a
          target="_blank"
          href="bronvermelding/#1">1</a
        >][<a target="_blank" href="bronvermelding/#2">2</a>]. Deze wet is in
        2020 aangenomen en zal van kracht gaan na 3 jaar. Dit zal pas over 3
        jaar van kracht gaan omdat er een aantal problemen zijn volgens de
        scholen. Ze werpen tegen dat ze bijvoorbeeld te weinig gymleraren,
        sporthallen of sportvelden hebben [<a
          target="_blank"
          href="bronvermelding/#2">2</a
        >]. Dit wordt bevestigd door een onderzoek dat uitgevoerd is in gemeente
        Tilburg. Hier zijn gedurende gemeentelijke sporthallen het hele jaar
        voor 43 procent van de tijd bezet; bij de gymzalen is dat voor 28
        procent van de tijd [<a target="_blank" href="bronvermelding/#3">3</a>].
        Dit lijkt misschien laag te zijn, alleen worden deze hallen gebruikt
        tijdens de uren wanneer het sportgebruik doorgaans plaatsvindt
        (doordeweeks in de middag en avond en in het weekend) waardoor ze tegen
        een organisatorische grens aan zitten [<a
          target="_blank"
          href="bronvermelding/#3">3</a
        >]. Om ervoor te zorgen dat er meer sport ruimte komt zullen wij naar
        buiten gaan kijken. Daarom zullen wij ons op de basisschool kinderen
        gaan richten zodat ze 2 uur per week buiten kunnen sporten met een
        nieuwe toestel. De 2 uur sporten zorgt voor een ‘gezonde school’.
        Hierdoor zijn leerlingen gezonder, leveren betere prestaties, stoppen ze
        minder snel met school en maken ze gezondere keuzes in het leven waar ze
        later profijt van zullen hebben. Verder is hierdoor het lesgeven
        interessanter, verloopt het leerproces beter voor medewerkers. Zo zegt
        Janette Kuipers(directeur OBS De Hasselbraam in Heerhugowaard ) “Ik
        ervaar in vergelijking met vijf jaar terug echt een beter pedagogisch
        klimaat”.
      </p>
      <p>
        Verder hadden we nog een aantal onderwerpen in onze muurkant
        opgeschreven waar we niet voor gekozen hebben. Een van deze punten was
        de aan tal blessures binnen het beweegonderwijs. 11% van de
        sportblessures bij de spoedeisende hulp zijn namelijk veroorzaakt
        tijdens het beweegonderwijs [<a target="_blank" href="bronvermelding/#4"
          >4</a
        >]. Dit hadden we bij onze stakeholder neergelegd alleen kregen hier
        geen positieve reactie op. Op deze manier zouden we een bestaand product
        gaan aan passen. De stakeholder zou eerder een nieuw product willen
        zien. Verder zijn wij erachter gekomen dat de ventilatie niet goed
        genoeg is en dat de temperaturen te hoog zijn in sporthallen. Alleen
        leek het ons een beter idee om te richten op het sporten buiten
        aangezien Bosan zich niet direct bezig houdt met het klimaat binnen een
        sporthal.
      </p>
    </div>
    <div class="section moscow" id="moscow">
      <h1>Moscow Methode</h1>
      <p>Tijdens het gebruiken van de Moscow methode wordt er gekeken naar welke onderdelen een product belangrijk zijn. Met deze methode krijg je een goede kijk op het te ontwerpen product. Dit is een wijze van prioriteiten stellen. Op deze manier zul je minder snel de overbodige punten van een product gaan uitwerken. Het is een afkorting, waarvan de letters staan voor: </p>
      <ul>
        <li>M - Must Haves: deze eisen (requirements) moeten in het eindresultaat terug komen, zonder deze eisen is het product onbruikbaar.</li>
        <li>S - Should Haves: deze eisen zijn zeer gewenst, maar zonder is het product wel bruikbaar.</li>
        <li>C - Could Haves: deze eisen zullen alleen aan bod komen als er tijd genoeg is.</li>
        <li>W - Won't Haves: : deze eisen zullen in dit project niet aan bod komen maar kunnen in toekomst wel interessant zijn.</li>
      </ul>
      <p>De MOSCOW methode is uitgewerkt in een Bijlage. Zie hieronder de bijlage. </p>
      
    </div>
    <a style="margin-bottom: 20px;" href="brainstorms" class="button"
      >Ga naar de volgende pagina</a
    >
  </div>
  <div class="right-bar">
    <TimelineSprint1 />
  </div>
</main>


<style>
  p {
    margin-top: 0;
  }
</style>
