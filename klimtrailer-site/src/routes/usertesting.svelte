<script>
  import TimelineSprint3 from "$lib/TimelineSprint3.svelte";
  import SlideShow from "$lib/SlideShow.svelte";
  import Mural from "$lib/Mural.svelte";

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

  let klimtrailerPhotos = [
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
  ];

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
    },
  ];

  let prototype4Photos = [
    {
      path: "images/prototype4/1.jpeg",
      alt: "3d Geprint Prototype 4-1",
    },
    {
      path: "images/prototype4/2.jpeg",
      alt: "3d Geprint Prototype 4-2",
    },
    {
      path: "images/prototype4/3.jpeg",
      alt: "3d Geprint Prototype 4-3",
    }
  ]
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
      <p style="color: #4491DA;">
        Hier zal er verteld worden hoe we ons idee getest hebben en welke
        veranderingen we door deze testen door gevoerd hebben en hoe deze
        onderbouwd zijn.
      </p>
      <p>
        Gedurende het hele ontwerpproces wordt er in een vroeg stadium al
        gewerkt aan een prototype. De eerste prototypen zullen zeer basic zijn.
        Het prototype is ervoor bedoelt om een weergave te geven van het idee.
        Met een prototype kun je het idee visualiseren bij een belanghebbend
        persoon. Omdat de groep niet op één lijn lag hoe het product nu het
        beste kon worden ontworpen is er eerst een brainstormsessie gestart met
        een basis schets. Hierbij heeft iedereen in de projectgroep een
        tekenblad gekregen. Vervolgens moest iedereen een tekening maken hoe zij
        het product in gedachten hadden. Hieruit zijn alle ideeschetsen
        uitgelegd geworden aan de groep. Vervolgens is er op één idee verder
        gegaan.
      </p>

      <p style="color: #F06119; display: inline;">De basisprincipes</p>
      <p>
        De 10 basisprincipes van prototypen. Dit zijn de heilige basisregels.
        Deze zijn zeer van belang anders kan een prototype niet het gewenste
        effect vervullen. Het aller belangrijkste basis principe is het eerste:
        “Maak het visueel en tastbaar”. Je leert sneller door in een vroeg
        stadium vaker te falen. Dit zijn juist de beste leermomenten van je
        ontwerp proces. Er moeten veel verschillende iteraties worden gedaan.
        Het is helaas praktisch onmogelijk om een levensecht werkend model te
        prototypen omdat het simpelweg gewoon teveel tijd kost en er geen budget
        voor is.
      </p>
      <img
        style="width: 100%;"
        src="/images/prototyping.png"
        alt="De 10 basisprincipes"
      />

      <p style="color: #F06119; display: inline;">
        In een vroeg stadium testen
      </p>
      <p>
        Het product moet in een vroeg stadium al worden tentoongesteld aan
        zoveel mogelijk mensen. Je moet ook zeker niet in je eerst idee blijven
        hangen. Het kan ook een volledig andere kant op gaan. Een product
        volledig uitwerken tot in detail en er volgens achter komen dat het niet
        bij de doelgroep past wordt op deze manier uitgesloten.
      </p>
      <p>
        De persona’s hebben hier ook een belangrijke rol. Je gaat de bril
        opzetten van een persona en nadenken wat zou deze persoon juist willen,
        of waar let deze persoon juist op. Voorafgaand aan het prototypen moet
        er gestart worden met het invullen van een prototype report card.
        Hierbij ga je van tevoren nadenken hoe je het prototype gaat
        ontwikkelen. Hierbij wordt er gestart met het bedenken van een naam voor
        het prototype. Vervolgens worden er drie kritische vragen gesteld,
        hiermee bepaal je de key metrics of success. Er zijn ook meerdere
        testmethodes bij één prototype. Zoals bijvoorbeeld een A/B test of een
        observatie. Het meest belangrijke bij de report card is eigenlijk welke
        aannames stellen we nu vast. Hierdoor hoeft daar geen rekening mee
        worden gehouden en is dit logischerwijs aanwezig.
      </p>

      <p style="color: #F06119; display: inline;">Eerste prototype</p>
      <p>
        Het eerste prototype moet basic der basic worden. Een simpele vorm van
        magneetjes op een whiteboard die een klimwand voorstelt kan al voldoen
        als een basic prototype. Het eerste prototype is in een korte tijdsduur
        van één uur gemaakt. Dit is een karton model geworden. Zie 3.1 Prototype
      </p>
      <p>
        Hierbij is er letterlijk een ‘’houtje-touwtje” model gemaakt. Het
        bestaat uit basis van karton en een touw die het mechanisme weergeeft.
        Een vervolg prototype is een groter karton model. Hierbij is er een
        plaat van 2 meter hoog bij 1 meter breed gebruikt. Hierbij zijn simpel
        gaten in het karton gemaakt. Deze moeten handgrepen voorstellen. Op deze
        manier kan er op een simpele manier het idee worden getest.
      </p>
      <SlideShow photos={prototype1Photos} id="1" />

      <p style="color: #F06119; display: inline;">3D model prototype</p>
      <p>
        Het prototype is ook in een 3d programma gemaakt. Hierbij kunnen
        makkelijk aanpassingen worden gedaan. Er is ervoor gekozen om een
        maquette te maken. Dit is gedaan door gebruik te maken van een 3d
        printer. Onderdeel per onderdeel is uitgeprint en vervolgens is dit met
        behulp van een scharnier en lijm vastgezet. Met deze toepassing kan de
        maquette duidelijk weergeven hoe het product werkt.
      </p>

      <SlideShow photos={prototype2Photos} id="2" maxwidth="300" />

      <p style="color: #F06119; display: inline;">Verdere ontwikkeling</p>
      <p>
        Toch blijft een hand schets het beste als een “quick prototype”. Hiermee
        kun je aan een persoon je idee weergeven. Tijdens een gesprek van de
        persona’s met Mark Janssen (van Fontys) is tevens ook het ontwerp laten
        zien. Hierbij heeft Mark gezegd of het niet makkelijker is dat de val
        mat meteen bij het product aanwezig is. Hieruit volgde een handschets in
        samenwerking met Mark. Dit was een derde evolutie van het ontwerp.
      </p>

      <p style="color: #F06119; display: inline;">Verplaatsbaar</p>
      <p>
        Er is ook het idee ontstaan om het product verplaatsbaar te maken. Dit
        is simpel weg gedaan door er wielen onder te plaatsen. Zo kan dit later
        makkelijk met een B rijbewijs worden vervoerd.
      </p>

      <SlideShow photos={klimtrailerPhotos} id="5" />

      <p style="color: #F06119; display: inline;">
        De evolutie van het prototype
      </p>
      <p>
        Bij het eerste prototype (1.0) zijn de wanden vast aan het product. De
        wanden konden in eerste instantie niet worden gekanteld. Bij het hierop
        volgende prototype (2.0) zijn de wanden demonteerbaar en kunnen ze van
        kantelhoek worden veranderd. Ook kwam er ter sprake dat het model
        makkelijk verplaatsbaar moet zijn. Hierdoor zijn er wielen onder gemaakt
        op de manier van een aanhanger. Bij het volgende prototype (3.0) is er
        in het middenstuk een klimrek gemaakt (zie foto prototypes). Op deze
        manier kun je er makkelijker overheen klimmen. Zo hoef je niet weer
        dezelfde richting terug op. Bij het laatste prototype (4.0) is het nog
        mogelijk om een optionele trampoline wand toe te voegen. Dit wordt
        gecombineerd met een luchtkussen. Op deze manier kan het product
        veelzijdig worden gebruikt en zorgt dit voor de meeste uitdaging. De
        prototypes zijn door iedere keer nieuwe inzichten te halen uit
        voornamelijk interview en brainstormsessies iedere keer veranderd. Er
        zijn meerdere ideeën bedacht per prototype. Iedere keer is er gekeken of
        de mogelijke toevoeging wel echt meerwaarde brengt aan het product. De
        basisschoolkinderen gebruiken eenmaal het product.
      </p>

      <SlideShow photos={prototype4Photos} id="4" />


      <p style="color: #F06119; display: inline;">Prototype testen</p>
      <p>
        We hebben dit ontwerp aan verschillende docenten van de sporthogeschool
        laten zien. Hierbij hebben we gepeild of het duidelijk is wat ons
        product doet en of het aan hun eisen zou voldoen. Uit deze momenten
        hebben we veel feedback gepakt die we uiteindelijk door verwerkt hebben
        in ons eindproduct.
      </p>
      <p>
        Ook hebben we ons prototype meegenomen naar de observatie van de
        basisschool gymles. We hebben het prototype aan de kinderen laten zien
        om te kijken of zij het er leuk uit vonden zien en of ze er interesse in
        hadden.
      </p>
    </div>

    <div class="section testenleerkaarten" id="testenleerkaarten">
      <h1>Testen met test en leerkaarten</h1>
      <p>
        Het doel van test en leerkaarten is om te beschrijven hoe we willen
        onderzoeken of ons product goed valt bij de docenten/mensen die er mee
        moeten werken. Deze kaarten helpen ook om ons product beter te valideren
        en daarmee de succeskansen te vergroten.
      </p>

      <p style="color: #F06119; display: inline;">Validatie</p>
      <p>
        Het idee was om het product te valideren bij docenten en eventuele
        aanmerkingen die er missen of over het hoofd gezien zijn in kaart te
        brengen. Om dit te doen is er aan meerdere vakdocenten en experts het
        product gedemonstreerd en is er hiermee een reactie uitgelokt. Ook
        zullen er een aantal interviews worden gegeven met als doel om te meten
        hoeveel potentie te zien is in de boulder mini. Als criteria is er
        aangegeven dat die voldoet zodra een docent potentie ziet in het
        product.
      </p>

      <p style="color: #F06119; display: inline;">Conclusie</p>
      <p>
        Uit dit onderzoek is gebleken dat er veel potentie zit in het idee, maar
        dat er nog veel veranderd moest worden of naar bepaalde dingen gekeken
        moet worden. Hierbij moet er gekeken worden naar de wetten van
        speel/sporttoestellen en de regelgeving van aanhangers. Ook is er als
        feedback gekomen dat het product multi inzetbaar moet zijn en niet
        alleen als een wand waar je op kan klimmen. Een aantal veranderingen
        waarnaar gekeken moet worden is dat er dikkere matten gebruikt moeten
        worden. Geen lampjes om de grepen, maar juist een volledige kleur. Er
        moet niet alleen twee maar vier zijdes gebruikt worden en de muur
        opklapbaar te maken voor meer variatie.
      </p>

      <Mural
        title="Frames"
        src="https://app.mural.co/embed/b8e9bc5e-afb5-47de-a82f-8e8a1c9ea1af"
      />
    </div>

    <div class="section prototypereportcard" id="prototypereportcard">
      <h1>Prototype Report Card</h1>
      <p style="color: #F06119; display: inline;">Prototype Report Card</p>
      <p>
        Zodra wij eenmaal hebben geprototyped was het tijd om naar buiten te
        gaan en feedback te ontvangen van mensen. Wij hebben het prototype
        report card ingezet om duidelijk te krijgen waar wij onderzoek naar
        moeten doen en hoe we dat moeten doen. Verder hebben wij een maar
        belangrijke criteria opgeschreven waar wij het succes van ons prototype
        aan kunnen meten.
      </p>

      <p style="color: #F06119; display: inline;">Aannames</p>
      <p>
        Ook neem je bepaalde aannames aan wat je verwacht dat het eindproduct
        aan zal voldoen. Zodra dit was opgesteld zijn wij op pad gegaan om onze
        aannames te valideren. Hieruit hadden wij geleerd dat veiligheid een erg
        belangrijk item is. Ook moest er gekeken worden naar de grootte van de
        handgrepen per leeftijd groep, nu ligt de focus op basisschoolkinderen
        dus is er alleen naar deze groep gekeken. Zodra hij uitgebreid zou
        worden naar hogere leeftijden zal hier opnieuw naar gekeken moeten
        worden. Verder was het idee om er een aanhanger van te maken dus moesten
        wij onderzoek gaan doen naar de wetgeving van aanhangers. Op basis van
        wat wij hebben geleerd moesten wij een aantal dingen veranderen of
        verder onderzoeken. Zo moesten wij de grepen anders maken dat voorheen
        en kwamen wij erachter dat de mensen die wij gesproken hadden wilden dat
        het prototype meer kon dan alleen een klimwand zijn, hierop zijn wij
        gaan brainstormen en hebben wij verschillende ideeën bedacht. Ook kregen
        wij de opmerking dat het product vergroot moest worden zodat het ook
        uitdagend was voor hogere leeftijden, dus een vergrote versie ons
        product.
      </p>
      <Mural
      title="Prototype Report Card"
      src="https://app.mural.co/embed/44028696-a1cc-4233-a470-eacf9d1b752d"
      />
    </div>

    <div class="section test-basisschool" id="test-basisschool">
      <h1>Test Basisschool de Kinderboom</h1>
      <p>TEST BASISSCHOOL DE KINDERBOOM</p>
      <p>LINK NAAR ALLE VOLLEDIG UITGEWERKTE TESTEN</p>
    </div>
    
    <a href="personas" class="button"
      >Ga naar de volgende pagina</a
    >
  </div>
  <div class="right-bar">
    <TimelineSprint3 />
  </div>
</main>

<style>
  main{
    display: flex;
    justify-content: center;
  }

  .content{
    width: 50%;
  }

  @media(min-width: 1350px){
    .right-bar{
      display: block;
    }
  }

  @media(max-width: 1349px){
    .right-bar{
      display: none;
    }

    .content{
      width: 65%;
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

  .right-bar{
    width: 566px;
  }


  p {
    margin-top: 0;
  }
</style>
