<script>
  import Mural from "$lib/Mural.svelte";
  import SlideShow from "$lib/SlideShow.svelte";
  import TimelineSprint2 from "$lib/TimelineSprint2.svelte";

  let schetsFotos = [
    {
      path: "images/schetsfotos/schets1.jpg",
      alt: "Schets 1",
    },
    {
      path: "images/schetsfotos/schets2.jpg",
      alt: "Schets 2",
    },
    {
      path: "images/schetsfotos/schets3.jpg",
      alt: "Schets 3",
    },
    {
      path: "images/schetsfotos/schets4.jpg",
      alt: "Schets 4",
    },
    {
      path: "images/schetsfotos/schets5.jpg",
      alt: "Schets 5",
    },
  ];
</script>

<svelte:head>
  <title>Brainstorms</title>
</svelte:head>

<div>
  <img
    src="images/Brainstorm.jpg"
    alt="woordenlijst"
    width="100%"
    style="height: 400px; object-fit: cover; position: relative;"
  />
  <span
    style="background-color: white; position: absolute; top: 440px; right: 0px;"
    ><p style="margin: 0 2px;">
      Foto by <a href="https://unsplash.com/@epicantus" target="blank"
        >Daria Nepriakhina</a
      >
      on <a href="https://unsplash.com/" target="blank">Unsplash</a>
    </p></span
  >
</div>

<main>
  <div class="left-bar" />
  <div class="content">
    <h1>Brainstorms</h1>
    <div class="section cimo" id="cimo">
      <h1>CIMO Analyses</h1>
      <p>
        Een CIMO analyse bestaat uit 4 delen zoals afgebeeld in de foto hier
        onder.
      </p>
      <img style="width: 60%;" src="/images/CIMO.jpg" alt="CIMO" />
      <p>
        Vanaf sprint 2 hebben we voor iedere sprint deze analyse ingevuld.
        Hierdoor hebben wij ons doel per sprint beter voor ogen en hebben we al
        nagedacht over de stappen die we moeten doorlopen om ons doel te halen.
        Hieronder staat de mural waar al onze CIMOs van het project staan.
      </p>
      <Mural
        title="CIMOs"
        src="https://app.mural.co/embed/b00af80c-18cd-4182-8a31-160205b9a1eb"
      />
    </div>
    <div class="section brainstorm" id="brainstorm">
      <h1>Brainstorm</h1>
      <p style="color: #F06119; display: inline;">De start</p>
      <p>
        Aan het begin van het proces is er gebruik gemaakt van
        brainstormsessies. Hier zijn verschillende vormen voor gebruikt, dit is
        gedaan om tot zoveel mogelijk ideeën te komen. Allereerst is gebruik
        gemaakt van een dieren brainstorm, deze manier zorgde ervoor dat op een
        hele andere manier naar het vraagstuk gekeken werd. Hierop volgde een
        brainstorm vorm aan de hand van het alfabet, deze manier hielp bij het
        bedenken van ideeën waar in eerste instantie niet aan gedacht werd.
      </p>
      <p style="color: #F06119; display: inline;">Tekenen werkt beter</p>
      <p>
        Deze twee vormen resulteerde in verschillende ideeën, maar er kwamen nog
        geen baanbrekende ideeën uit. Dit was de reden dat de superhelden
        brainstormmethode gebruikt werd. Hier kwamen al betere ideeën uit, wat
        opviel was dat er aantal waren die gingen tekenen in plaats van typen.
        Al snel werd duidelijk dat tekenen een veel duidelijk beeld gaf en ook
        tot veel meer ideeën leidde.
      </p>
      <p>
        Toen het bleek dat tekenen tot succesvollere ideeën leidde, is er de
        keuze gemaakt om alleen nog maar te tekenen tijdens de
        brainstormsessies.
      </p>

      <SlideShow photos={schetsFotos} id="7" />

      <p style="color: #F06119; display: inline;">Het idee</p>
      <p>
        Na meer dan honderdvijftig ideeën bedacht te hebben is er aan de hand
        van een MOSCOW gekeken welke ideeën origineel waren en hierbij
        potentieel het vraagstuk zouden oplossen. Hier kwam uiteindelijk het
        free run parcour uit, iedereen was het erover eens, dit was een goed
        maar ook innovatief idee.
      </p>
      <p>
        Dit idee is voorgelegd aan Bosan en ook zij waren positief, helaas werd
        ook verteld dat dit idee al bestond. Sterker nog, dit idee stond sinds
        een week in de showroom, we waren dus op de goede weg, alleen waren we
        net te laat.
      </p>
      <p>
        Toen is er samen met Bosan gekeken naar de andere WOW ideeën. Al snel
        kwam hier de Boulder Mini bij naar voren. Iedereen vond ook dit een goed
        en innovatief idee, hier is dus ook verder op doorgeborduurd.
      </p>
      <p>
        Uiteindelijk is hier ook een ideefiche van gemaakt om het idee concreet
        te maken.
      </p>
      <p style="color: #F06119; display: inline;">Verschillende wanden</p>
      <p>
        Na enige tijd bezig te zijn geweest met de Boulder Mini kwamen er
        geluiden dat de Boulder Mini wellicht ook voor anderen dingen inzetbaar
        zou moeten zijn. Om dit te realiseren is er een brainstormsessie
        geweest, het bleek namelijk dat iedereen meer kansen zag in de Boulder
        Mini dan alleen een Boulderwand. Om nog meer, en ook van anderen inbreng
        te krijgen is een brainstormsessie samen met de Vitality Hub gedaan. Dit
        was de meest effectieve manier om alle ideeën op tafel te krijgen en zo
        de beste uit te kunnen kiezen. Naar aanleiding van deze sessie is ook
        het concept van de verschillende wanden ontstaan.
      </p>
      <p>
        Hieronder de mural die we tijdens al onze brainstorms hebben gebruikt:
      </p>
      <Mural
        title="Brainstorm"
        src="https://app.mural.co/embed/2551f8da-bf76-45d8-874a-3ae60cb5103a"
      />
    </div>
    <div class="section frames" id="frames">
      <h1>Frames</h1>
      <p style="color: #F06119; display: inline;">Het maken van frames</p>
      <p>
        Om ons probleem vanuit meerdere hoeken te bekijken hebben we gebruik
        gemaakt van frames, deze frames zijn ontstaan vanuit de DESTEP. Ieder
        frame hebben we een bijpassende naam gegeven die duidelijk aangeeft waar
        het over gaat. Vervolgens is het frame beschreven en is er bekeken wat
        de waarde propositie zou zijn van het frame. Onderaan het frame is het
        probleem kernachtig neergezet en is al meteen gekeken naar een
        oplossingsrichting, hierbij is ook gelijk breed gekeken naar
        alternatieven. De bedoeling is dat de frames niet vaststaan vanaf het
        begin, hier kan gedurende het ontwerpproces een evaluatie in plaats
        vinden.
      </p>
      <p style="color: #F06119; display: inline;">Onze frames</p>

      <p>
        Aan het begin van de minor waren er dan in eerste instantie 3 frames:
        Minimaal 2u gym, Buiten gymmen, Opberging en Motivatie. Er is
        uiteindelijk verdergegaan met de eerste 2 frames, hier leek de meeste
        potentie in te zitten. Achteraf leken deze frames in essentie veel op
        elkaar, vandaar dat deze zijn samengevoegd tot één frame. Met dit frame
        zijn we ook verdergegaan en zijn de eerste ideeën ontstaan.
      </p>
      <p>Hieronder de mural waar onze frames zijn uitgewerkt:</p>
      <Mural
        title="Frames"
        src="https://app.mural.co/embed/27e91e81-af67-4650-ae4c-dc59a218d101"
      />
    </div>

    <a href="usertesting" class="button">Ga naar de volgende pagina</a>
  </div>
  <div class="right-bar">
    <TimelineSprint2 />
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
