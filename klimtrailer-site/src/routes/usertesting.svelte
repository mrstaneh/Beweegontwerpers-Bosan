<script>
  import TimelineSprint1 from "$lib/TimelineSprint1.svelte";
  import SlideShow from "$lib/SlideShow.svelte";

  let prototype1Photos = [
    {
      path: "images/prototype1/2-Karton.jpg",
      alt: "Kartonnen Prototype 1",
    },
    {
      path: "images/prototype1/3-Karton.jpg",
      alt: "Kartonnen Prototype 2",
    },
    {
      path: "images/prototype1/4-Karton.jpg",
      alt: "Kartonnen Prototype 3",
    },
    {
      path: "images/prototype1/5-Karton.jpg",
      alt: "Kartonnen Prototype 4",
    },
  ];

  /*let klimtrailerPhotos = [
    {
      path: "images/klimtrailer-slideshow/klimtrailer1.png",
      alt: "klim1",
    },
    {
      path: "images/klimtrailer-slideshow/klimtrailer2.png",
      alt: "klim2",
    },
    {
      path: "images/klimtrailer-slideshow/klimtrailer3.png",
      alt: "klim3",
    },
    {
      path: "images/klimtrailer-slideshow/klimtrailer4.jpeg",
      alt: "klim4",
    },
  ];*/

  let prototype2Photos = [
    {
      path: "images/prototype2/schaalmodel1.jpg",
      alt: "3d Geprint Prototype 1",
    },
    {
      path: "images/prototype2/schaalmodel2.jpg",
      alt: "3d Geprint Prototype 2",
    },
    {
      path: "images/prototype2/schaalmodel3.jpg",
      alt: "3d Geprint Prototype 3",
    }
  ];
</script>

<svelte:head>
  <title>Usertesting</title>
</svelte:head>

<main>
  <div class="left-bar" />
  <div class="content">
    <h1>Usertesting</h1>
    <div class="section prototyping" id="prototyping">
      <h1>Prototyping</h1>
      moeten kopjes bij
      <p style="color: #4491DA;">Hier zal er verteld worden hoe we ons idee getest hebben en welke veranderingen we door deze testen door gevoerd hebben en hoe deze onderbouwd zijn.</p>
      <p>Gedurende het hele ontwerp proces wordt er in een vroeg stadium al gewerkt aan een prototype. De eerste prototypen zullen zeer basic zijn. Het prototype is ervoor bedoelt om een weergave te geven van het idee. Met een prototype kun je het idee visualiseren bij een belanghebbend persoon. Omdat de groep niet op één lijn lag hoe het product nu het beste kon worden ontworpen is er eerst een brainstorm sessie gestart met een basis schets. Hierbij heeft iedereen in de projectgroep een tekenblad gekregen. Vervolgens moest iedereen een tekening maken hoe zij het product in gedachten hadden. Hieruit zijn alle ideeschetsen uitgelegd geworden aan de groep. Vervolgens is er op één idee verder gegaan. </p>
      <p>Het product moet in een vroeg stadium al worden tentoongesteld aan zoveel mogelijk mensen. Je moet ook zeker niet in je eerst idee blijven hangen. Het kan ook een volledig andere kant op gaan. Een product volledig uitwerken tot in detail en er volgens achter komen dat het niet bij de doelgroep past wordt op deze manier uitgesloten. </p>
      <p>De persona’s hebben hier ook een belangrijke rol. Je gaat de bril opzetten van een persona en nadenken wat zou deze persoon juist willen, of waar let deze persoon juist op. Voorafgaand aan het prototypen moet er gestart worden met het invullen van een prototype report card. Hierbij ga je van te voren nadenken hoe je het prototype gaat ontwikkelen. Hierbij wordt er gestart met het bedenken van een naam voor het prototype. Vervolgens worden er drie kritische vragen gesteld, hiermee bepaal je de key metrics of success. Er zijn ook meerdere testmethodes bij één prototype. Zoals bijvoorbeeld een A/B test of een observatie. Het meest belangrijke bij de report card is eigenlijk welke aannames stellen we nu vast. Hierdoor hoeft daar geen rekening mee worden gehouden en is dit logischerwijs aanwezig. </p>
      <p>Het eerste prototype moet basic der basic worden. Een simpele vorm van magneetjes op een whiteboard die een klimwand voorstelt kan al voldoen als een basic prototype. Het eerste prototype is in een korte tijdsduur van één uur gemaakt  . Dit is een karton model geworden. Zie  3.1 Prototype</p>
      <p>Hierbij is er letterlijk een "houtje-touwtje" model gemaakt. Het bestaat uit basis van karton en een touw die het mechanisme weergeeft. Een vervolg prototype is een groter karton model. Hierbij is er een plaat van 2 meter hoog bij 1 meter breed gebruikt. Hierbij zijn simpel gaten in het karton gemaakt. Deze moeten handgrepen voorstellen. </p>
      <SlideShow photos={prototype1Photos} id=1 />
      <p>Het prototype is ook in een 3d programma gemaakt. Hierbij kunnen makkelijk aanpassingen worden gedaan.  Er is ervoor gekozen om een maquette te maken. Dit is gedaan door gebruik te maken van een 3d printer. Onderdeel per onderdeel is uitgeprint en vervolgens is dit met behulp van een scharnier en lijm vastgezet. Met deze toepassing kan de maquette duidelijk weergeven hoe het product werkt. </p>
      <SlideShow photos={prototype2Photos} id=2 maxwidth=300 />
      <p> Toch blijft een hand schets het beste als een “quick prototype”. Hiermee kun je aan een persoon je idee weergeven. Tijdens een gesprek van de persona’s met Mark (Fontys) is tevens ook het ontwerp laten zien. Hierbij heeft Mark gezegd of het niet makkelijker is dat de val mat meteen bij het product aanwezig is. Hieruit volgde een handschets in samenwerking met Mark. Dit was een derde evolutie van het ontwerp.</p>
      <p>We hebben dit ontwerp aan verschillende docenten van de sporthogeschool laten zien. Hierbij hebben we gepeild of het duidelijk is wat ons product doet en of het aan hun eisen zou voldoen. Uit deze momenten hebben we veel feedback gepakt die we uiteindelijk door verwerkt hebben in ons eindproduct.</p>
      <p>Ook hebben we ons prototype meegenomen naar de observatie van de basisschool gymles. We hebben het prototype aan de kinderen laten zien om te kijken of zij het er leuk uit vonden zien en of ze er interesse in hadden.</p>
      <p>De 10 basisprincipes van prototypen. Dit zijn de heilige basisregels. Deze zijn zeer van belang anders kan een prototype niet het gewenste effect vervullen. Het aller belangrijkste basis principe is het eerste: “Maak het visueel en tastbaar”. Je leert sneller door in een vroeg stadium vaker te falen. Dit zijn juist de beste leermomenten van je ontwerp proces. Er moeten veel verschillende iteraties worden gedaan. Het is helaas praktisch onmogelijk om een levensecht werkend model te prototypen omdat het simpelweg gewoon teveel tijd kost en er geen budget voor is.</p>
      <img style="width: 100%;" src="/images/prototyping.png" alt="De 10 basisprincipes"/>
    </div>
    <div class="section personas" id="personas">
      <h1>Personas</h1>
      <p style="color: #4491DA;">Hier zullen onze persona’s toegelicht worden. Dit zal gaan over de leraren en leerlingen. Je kunt de personas op <a href="/personas" target="_blank">deze</a> pagina vinden.</p>

      <p style="color: #F06119; display: inline;">De basis in het kort</p>
      <p>In het begin van het project zijn er meerdere persona’s ontstaan. Deze persona’s geven een duidelijke weergave van onze doelgroep.</p>

      <p style="color: #F06119; display: inline;">Voordelen</p>
      <p>Een voordeel van de persona’s is dat je vanuit die persoon kunt ontwerpen. Je gaat dus echt een persona bril opzetten. Tevens staat een persona niet vast. Een persona zal voortdurend evolueren.</p>

      <p style="color: #F06119; display: inline;">Validatie</p>
      <p>Een ander belangrijk punt is dat er een validatie moet zijn. Dit is gedaan door onder andere de persona’s te presenteren aan Anoek. Zij heeft gekeken of de persona’s pasten bij een stereotype basisschoolkind. Hierbij gaf Anoek aan dat er tevens veel verschillende basisschoolkinderen zijn         . Het is ook mogelijk dat je een persona afstoot. Sommige persona’s zijn van meerwaarde op het ontwerpproces. Hierbij is iedere persona afgegaan en is er gekeken wat er belangrijk is bij het product. 
        Daarnaast is er meermaals feedback gevraagd op onze persona’s door Mark Janssen. Dankzij deze feedback konden onze persona’s telkens relevanter gemaakt worden. Uiteraard hebben diverse interviews en schoolbezoeken ons ook erg geholpen bij het creëeren van geloofwaardige persona’s.
        </p>

        <p style="color: #F06119; display: inline;">Onderbouwing keuzes in proces naar aanleiding van de persona's</p>
        <p>Tijdens het proces zijn er belangrijke keuzes gemaakt aan de hand van de persona’s. een aantal van deze keuzes zijn hieronder uitgelicht en onderbouwd.</p>
        <p>De persona’s die het meest bepalend zijn geweest voor het proces zijn Rafaël, Nicky, Luca en Amy. Hun karaktereigenschappen hebben voor het overgrote deel gezorgd voor toevoegingen aan de Boulder Mini. Al deze toevoegingen zijn er om de Boulder Mini voor iedereen zo goed als mogelijk te laten voldoen aan hun wensen. </p>
        <p>Aan het begin van het ontwerpproces zijn er verschillende interviews gehouden met verschillende experts. Tijdens deze interviews kwam al snel naar voren dat docenten toestellen vaak ook op andere manieren gebruiken dan alleen daar waar ze voor bedoeld zijn. Joris is één van deze docenten en gebruikt tijdens zijn les de toestellen vaak op een creatieve manier. Joris heeft er dus voor gezorgd dat de Boulder Mini niet alleen te gebruiken is als klimmuur maar ook toepasbaar moet zijn op andere manieren. </p>
        <p>Er zitten veel positieve kanten aan een creatieve instelling, deze moeten dus ook gestimuleerd worden. Naar aanleiding hiervan is er dus nagedacht over mogelijkheden om dit te realiseren, hier kwam het idee uit om verschillende wanden te bedenken. Dit zorgt ervoor dat de Boulder Mini veelzijdiger is en stimuleert daarmee ook de creatieve kant van de docenten.</p>
        <p>Aansluitend hierop is het ook de bedoeling dat de kinderen voldoende nieuwe dingen leren tijdens de les. Voor de docenten is het dus ook van belang dat er voldoende en verschillende leerlijnen worden geraakt met de Boulder Mini, dit is met name voor Marc en Nicky heel belangrijk.</p>
        <p>Verder vinden Nicky en de andere docenten het heel belangrijk dat er verschillende niveaus mogelijk moeten zijn bij het gebruik van de Boulder Mini. Dit omdat er dan op veel verschillende niveaus les gegeven kan worden. Enerzijds om ervoor te zorgen dat alle kinderen mee kunnen doen en anderzijds om te zorgen dat alle kinderen constant opnieuw uitgedaagd worden. 
          Maar niet alleen voor de docenten was dit een eis, ook voor de kinderen is het belangrijk dat er verschillende niveaus mogelijk zijn. Hierdoor zullen ze zich niet buitengesloten voelen omdat ze allemaal mee kunnen doen en zullen ze gemotiveerd blijven omdat ze steeds opnieuw uitgedaagd worden.
          </p>
          <p>Een nieuw toestel zorgt logischerwijs voor een hoop vragen. Het is dan ook heel belangrijk dat de docenten het nieuwe toestel goed leren kennen en gebruiken. Hierbij is een handleiding noodzakelijk en ook een logische stap in het proces. Voor Amy in het bijzonder, zij heeft namelijk minder ervaring met toestellen en voor haar is het dan ook een eis dat de Boulder Mini simpel en veilig te gebruiken is. </p>
          <p>Om goed af te sluiten is er ook al nagedacht over de toekomst. Een mooie eventuele toevoeging zou zijn om verlichting in de grepen te verwerken. Met deze optie krijg je nog meer mogelijkheden om de verschillende routes uit te zetten en op deze manier wordt het dus nog makkelijker om de route aan te passen aan het kind. Dit zou met name voor Luca en Mariec een toevoeging zijn. </p>
          <p style="font-style: italic;">Om goed af te sluiten is er ook al nagedacht over de toekomst. Een mooie eventuele toevoeging zou zijn om verlichting in de grepen te verwerken. Met deze optie krijg je nog meer mogelijkheden om de verschillende routes uit te zetten en op deze manier wordt het dus nog makkelijker om de route aan te passen aan het kind. Dit zou met name voor Luca en Mariec een toevoeging zijn. </p>
          <p style="font-style: italic;">Verder zou met deze verlichting ook gedacht kunnen worden aan het gevoel van succes. Voornamelijk Luca en Rafaël zouden hier profijt van hebben. Zij zijn gemotiveerder als ze worden aangemoedigd en deze eventuele verlichting zou hierbij helpen.</p>
    </div>
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