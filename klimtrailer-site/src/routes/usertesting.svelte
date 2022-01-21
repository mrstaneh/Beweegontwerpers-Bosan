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
    },
  ];
</script>

<svelte:head>
  <title>Usertesting</title>
</svelte:head>

<div>
  <img
    src="images/Prototyping.jpg"
    alt="woordenlijst"
    width="100%"
    style="height: 400px; object-fit: cover; position: relative;"
  />
  <span
    style="background-color: white; position: absolute; top: 440px; right: 0px;"
    ><p style="margin: 0 2px;">
      Foto by <a href="https://unsplash.com/@sigmund" target="blank"
        >Sigmund</a
      >
      on <a href="https://unsplash.com/" target="blank">Unsplash</a>
    </p></span
  >
</div>

<main>
  <div class="left-bar" />
  <div class="content">
    <h1>Usertesting</h1>
    <div class="section prototyping" id="prototyping">
      <h1>Prototyping</h1>
      <p style="color: #4491DA;">
        Hier zal er verteld worden hoe het idee getest is, welke veranderingen
        door deze testen doorgevoerd zijn en hoe deze onderbouwd zijn.
      </p>
      <p>
        Gedurende het hele ontwerpproces wordt er in een vroeg stadium al
        gewerkt aan een prototype, wel zullen de eerste prototypen zeer
        eenvoudig zijn. Het prototype is ervoor bedoelt om een weergave te geven
        van het idee, hiermee kun je het idee visualiseren bij een belanghebbend
        persoon.
      </p>
      <p>
        Omdat de groep niet op één lijn lag hoe het product nu het beste kon
        worden ontworpen is er eerst een brainstormsessie gedaan met een basis
        schets. Hierbij heeft iedereen in de projectgroep een tekenblad
        gekregen. Vervolgens moest iedereen een tekening maken hoe zij het
        product in gedachten hadden en heeft iedereen zijn schets uitgelegd aan
        de rest. Uiteindelijk is er keuze gemaakt en is er met één idee verder
        gegaan.
      </p>

      <p style="color: #F06119; display: inline;">
        In een vroeg stadium testen
      </p>
      <p>
        Het product moest in een vroeg stadium al worden tentoongesteld aan
        zoveel mogelijk mensen. Op deze manier is er direct sprake van feedback
        en wordt gelijk duidelijk of er behoefte is aan het idee. Hiermee wordt
        voorkomen dat een product volledig uitgewerkt wordt, om er dan later
        achter te komen dat het niet bij de doelgroep past. Daarbij komend moet
        ook nooit in het eerste idee gehangen blijven worden.
      </p>
      <p>
        De persona’s spelen hier ook een belangrijke rol in. Je gaat de bril
        opzetten van een persona en bedenken wat deze persoon zou willen of waar
        deze persoon juist op let. Voorafgaand aan het prototypen moet er
        gestart worden met het invullen van een prototype report card. Hierbij
        ga je van tevoren nadenken hoe je het prototype gaat ontwikkelen. Als
        eerst wordt er een naam bedacht voor het prototype. Vervolgens worden er
        drie kritische vragen gesteld, hiermee bepaal je de key metrics of
        succes. Ook is er sprake van meer dan één testmethode per prototype,
        zoals bijvoorbeeld een A/B test of een observatie. Het meest belangrijke
        wat duidelijk wordt aan de hand van de report card is welke aannames
        vastgesteld worden. Hier hoeft daar geen rekening meer mee gehouden te
        worden en spreekt dit voor zich.
      </p>

      <p style="color: #F06119; display: inline;">Eerste prototype</p>
      <p>
        Het eerste prototype moet zo eenvoudig mogelijk zijn. Een simpele vorm
        van magneetjes op een whiteboard die een klimwand voorstelt kan al
        voldoen als een eerste prototype. Het eerste prototype is in een korte
        tijdsduur van één uur gemaakt, dit is een karton model geworden. Zie 3.1
        Prototype
      </p>
      <p>
        Hierbij is er letterlijk een ‘’houtje-touwtje” model gemaakt, de basis
        bestaat uit karton en een touw die het mechanisme weergeeft. Een vervolg
        prototype is een groter karton model. Hierbij is er een plaat van 2
        meter hoog bij 1 meter breed gebruikt, hier zijn gaten in het karton
        gemaakt en deze stellen de grepen voor. Op deze manier kan het idee op
        een eenvoudige manier worden getest.
      </p>
      <SlideShow photos={prototype1Photos} id="1" />

      <p style="color: #F06119; display: inline;">3D model prototype</p>
      <p>
        Bij dit prototype is gekozen voor een maquette vorm. Het prototype is in
        een 3d programma gemaakt, hier kunnen indien nodig eenvoudig
        aanpassingen worden gemaakt. Elk onderdeel is uitgeprint met een 3d
        printer en is vervolgens met behulp van een scharnier en lijm vastgezet.
        Met deze toepassing kan de maquette duidelijk weergeven hoe het product
        werkt.
      </p>

      <SlideShow photos={prototype2Photos} id="2" maxwidth="300" />

      <p style="color: #F06119; display: inline;">Verdere ontwikkeling</p>
      <p>
        Toch blijft een hand schets het beste als een “quick prototype”. Hiermee
        kun je aan een persoon je idee weergeven. Tijdens een gesprek over de
        persona’s met Mark (van Fontys) is tevens ook het ontwerp laten zien.
        Hierbij vroeg Mark zich af of het niet eenvoudiger is als de val mat
        meteen bij het product toegevoegd is. Hieruit volgde een handschets in
        samenwerking met Mark, dit was een derde evolutie van het ontwerp.
      </p>

      <p style="color: #F06119; display: inline;">Verplaatsbaar</p>
      <p>
        Er is ook het idee ontstaan om het product verplaatsbaar te maken, dit
        is gerealiseerd door er wielen onder te plaatsen. Zo kan het later
        makkelijk door iemand met een B rijbewijs worden vervoerd.
      </p>

      <SlideShow photos={klimtrailerPhotos} id="5" />

      <p style="color: #F06119; display: inline;">
        De evolutie van het prototype
      </p>
      <p>
        Bij het eerste prototype (1.0) zitten de wanden vast aan het product en
        konden de wanden in eerste instantie niet kantelen.
      </p>
      <p>
        Bij het hierop volgende prototype (2.0) zijn de wanden demonteerbaar en
        kunnen deze wel van kantelhoek veranderd worden. Ook kwam er ter sprake
        dat het model makkelijk verplaatsbaar moet zijn, om deze reden zijn er
        wielen onder het prototype gemaakt, dit op dezelfde manier als bij een
        aanhanger.
      </p>

      <p>
        Bij het volgende prototype (3.0) is er in het middenstuk een klimrek
        gemaakt (zie foto prototypes). Op deze manier kun je er makkelijker
        overheen klimmen en hoef je niet weer dezelfde richting terug.
      </p>

      <p>
        Bij het laatste prototype (4.0) is het mogelijk geworden om
        verschillende optionele wanden toe te voegen. Zo is er een bijvoorbeeld
        trampoline wand bedacht, deze wordt gecombineerd met een luchtkussen. Op
        deze manier kan het product veelzijdig worden gebruikt en zorgt dit voor
        nog meer uitdaging.
      </p>

      <p>
        De prototypes zijn iedere keer veranderd, dit kwam door de nieuwe
        inzichten die opgedaan zijn tijdens interviews en brainstormsessies.
      </p>
      <p>
        Hieruit kwamen meerdere ideeën voor elk prototype. Bij elk van deze
        ideeën is er gekeken of de mogelijke toevoeging wel echt meerwaarde
        bracht aan het product. Dit is gedaan aan de hand van persona’s, zij
        zijn uiteindelijk degene die het product gaan gebruiken.
      </p>
      <SlideShow photos={prototype4Photos} id="4" />

      <p style="color: #F06119; display: inline;">Prototype testen</p>
      <p>
        Dit ontwerp is aan verschillende docenten van de sporthogeschool
        voorgelegd. Hierbij is gepeild of het duidelijk is wat het product doet
        en of het aan hun eisen zou voldoen. Uit deze momenten is veel feedback
        gehaald wat uiteindelijk verwerkt is in het eindproduct.
      </p>
      <p>
        Ook is het prototype meegenomen naar de observatie van de basisschool
        gymles. Het prototype is laten zien aan de kinderen om te kijken of zij
        het er leuk uit vonden zien en of ze er interesse in hadden.
      </p>

      <p style="color: #F06119; display: inline;">De basisprincipes</p>
      <p>
        Om op de juiste manier bezig te zijn met prototyping zijn er 10
        basisprincipes. Deze zijn zeer van belang anders kan een prototype niet
        het gewenste effect vervullen. Het allerbelangrijkste basisprincipe is
        de eerste: “Maak het visueel en tastbaar”. Ook leer je sneller door in
        een vroeg stadium regelmatig te falen. Dit zijn juist de beste
        leermomenten van je ontwerpproces. Verder moeten er veel verschillende
        iteraties worden gedaan.
      </p>
      <p>
        Helaas is het praktisch onmogelijk om een levensecht werkend model te
        prototypen, dit kost te veel tijd en er geen budget voor is.
      </p>
      <img
        style="width: 100%;"
        src="/images/prototyping.png"
        alt="De 10 basisprincipes"
      />
      <p>
        Voor meer fotos van de prototypes zie de <a
          href="/pdf-bijlage/prototype.pdf"
          target="_blank">foto bijlage</a
        >
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
        moeten doen en hoe we dat moeten doen. Verder hebben wij maar een
        belangrijke criteria opgeschreven waar wij het succes van ons prototype
        aan kunnen meten.
      </p>

      <p style="color: #F06119; display: inline;">Aannames</p>
      <p>
        Ook neem je bepaalde aannames aan wat je verwacht dat het eindproduct
        aan zal voldoen. Zodra dit was opgesteld zijn wij op pad gegaan en
        hebben wij mensen gesproken en gevraagd wat ze van ons prototype vinden.
        Hieruit hadden wij geleerd dat de veiligheid een erg belangrijk item is.
        Ook moest er gekeken worden naar de grootte van de handgrepen per
        leeftijd groep, nu ligt de focus op basisschoolkinderen dus is er alleen
        naar deze groep gekeken. Zodra hij uitgebreid zou worden naar hogere
        leeftijden zal hier opnieuw naar gekeken moeten worden. Verder was het
        idee om er een aanhanger van te maken dus moesten wij onderzoek gaan
        doen naar de wetgeving van aanhangers. Op basis van wat wij hebben
        geleerd moesten wij een aantal dingen veranderen of verder onderzoeken.
        Zo moesten wij de grepen anders maken dat voorheen en kwamen wij
        erachter dat de mensen die wij gesproken hadden wilden dat het prototype
        meer kon dan alleen een klimwand zijn, hierop zijn wij gaan brainstormen
        en hebben wij verschillende ideeën bedacht. Ook zei iemand dat die graag
        wou dat het prototype voor basisschoolkinderen vergroot moest worden
        naar ook hogere leeftijden, dus een grotere versie van het prototype te
        gaan maken.
      </p>
      <Mural
        title="Prototype Report Card"
        src="https://app.mural.co/embed/44028696-a1cc-4233-a470-eacf9d1b752d"
      />
    </div>

    <div class="section test-basisschool" id="test-basisschool">
      <h1>Test Basisschool de Kinderboom</h1>
      <p>
        Om onze doelgroep goed te leren kennen was het van belang dat we een
        keer langs zouden gaan bij een gymles, om te zien hoe kinderen
        tegenwoordig gymles krijgen (dit zou namelijk heel anders kunnen zijn
        ten opzichte van onze eigen ervaringen). Verder was het ook van belang
        om het product goed te kunnen testen, zodat we weten of de doelgroep wel
        zit te wachten op een boulderwand of buiten gymmen. Gelukkig kende Loes
        iemand via haar werk die gymles gaf op een aantal scholen, bij een van
        deze scholen mochten we langskomen: Basisschool de Kinderboom. We waren
        uitgenodigd om 3 lessen te observeren en tussendoor een aantal vragen te
        stellen aan de kinderen. Dit ging om de groepen 4, 7 en 8. Dus 2 van de
        groepen vielen goed in de doelgroep.
      </p>

      <p style="color: #F06119; display: inline;">Conclusie</p>
      <p>
        Tijdens het observeren is er vooral opgevallen dat de docent (vaak) in
        de ochtend alle onderdelen klaar zet die hij/zij zal behandelen met de
        kinderen van de meerdere groepen die les hebben die dag, dit bleek ook
        uit het gesprek met de gymdocent (Michelle). Om het wel uitdagend te
        houden voor de oudere kinderen worden de onderdelen natuurlijk
        moeilijker gemaakt of er wordt meer van een kind verwacht. Verder waren
        de kinderen erg enthousiast over de Boulder Mini en zouden ze het zeker
        leuk vinden om meer buiten te gymmen. Bij een aantal kinderen zag je al
        een glimlach ontstaan bij het idee om buiten te kunnen gymmen.
      </p>

      <p>
        Alle bovenstaande testen staan uitgewerkt in deze <a
          target="_blank"
          href="pdf-bijlage/prototype-test.pdf">bijlage</a
        >.
      </p>
    </div>

    <a href="personas" class="button">Ga naar de volgende pagina</a>
  </div>
  <div class="right-bar">
    <TimelineSprint3 />
  </div>
</main>

<style>
  main {
    display: flex;
    justify-content: center;
  }

  .content {
    width: 50%;
  }

  @media (min-width: 1350px) {
    .right-bar {
      display: block;
    }
  }

  @media (max-width: 1349px) {
    .right-bar {
      display: none;
    }

    .content {
      width: 65%;
    }
  }

  @media (max-width: 1299px) {
    .content {
      width: 75%;
    }
  }

  @media (max-width: 750px) {
    .content {
      width: 95%;
    }
  }

  .right-bar {
    width: 300px;
  }

  p {
    margin-top: 0;
  }
</style>
