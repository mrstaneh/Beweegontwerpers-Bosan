<script>
  let woordenlijst = [
    {
      word: 'Primair Onderwijs',
      description: 'Primair onderwijs is de overkoepelende sector voor het basisonderwijs én het speciaal basisonderwijs (SBO).'
    },
    {
      word: 'Stakeholder',
      description: 'Stakeholders zijn personen of groepen van personen die een direct of indirect belang hebben bij de organisatie en/of omgekeerd. Kortom alle belanghebbenden.'
    },
    {
      word: 'Boulderen',
      description: 'Boulderen is een discipline binnen de klimsport en betekent het klimmen van een korte route op een vaak dicht bij de grond gelegen echte of kunstmatige rots zonder het gebruik van een touw of andere vorm van zekering.'
    },
    {
      word: 'Beweegrichtlijnen',
      description: 'Geeft aan hoeveel beweging nodig is voor een goede gezondheid, van jong tot oud. Een belangrijk uitgangspunt wanneer je anderen stimuleert meer te bewegen voor een gezondere leefstijl.'
    },
    {
      word: 'Iteratief',
      description: 'Een iteratief proces wordt gekenmerkt door stelselmatige herhaling van onderdelen van het proces, zij het met instelbare, veranderlijke waarden, waardoor allerlei variaties en vertakkingen in het resulterende patroon kunnen optreden.'
    },
    {
      word: 'Incrementeel',
      description: 'Incrementeel betekent aangroeiend, toenemend. Bij een incrementeel proces lever je het eindproduct stapsgewijs op. Elk nieuw increment is een kleine toevoeging aan hetgeen er al was.'
    },
    {
      word: 'Leasen',
      description: "Leasing is een financieringsvorm die je gebruikt voor bedrijfsmiddelen. Denk aan bedrijfsauto's, machines, computers of kopieerapparaten. De leasemaatschappij financiert het bedrijfsmiddel en jij betaalt een maandelijks bedrag voor het gebruik."
    },
    {
      word: 'Validatie',
      description: "Validatie is het controleren van de waarde van een kenmerk of relatie van een geografisch object op geldigheid of juistheid ten opzichte van vastgestelde regels in een model."
    },
    {
      word: 'Beweegvignet',
      description: "Herkenningsplaatje voor een gezonde school."
    },
    {
      word: 'Multidisciplinaire groep',
      description: "Een multidisciplinair team is een groep mensen die allen gespecialiseerd zijn in een ander vakgebied en samenwerken aan een opdracht waarbij kennis in verschillende vakgebieden vereist is om de opdracht succesvol te voltooien."
    },
    {
      word: 'Alternatieven',
      description: "Een alternatief is een andere mogelijkheid of oplossing. Het kan ook 'afwijkend' of 'anders' betekenen. Wanneer iets niet lukt, wordt vaak gekeken naar andere opties: een alternatief."
    },
    {
      word: 'Visueel',
      description: "Iets wat je met het oog waarneemt."
    },
    {
      word: 'Prototype',
      description: "Een prototype is een vroeg model van een product, handgemaakt of via rapid prototyping, waarmee optredende krachten, de werking of passing van onderdelen wordt getest en de productie wordt voorbereid."
    },
    {
      word: 'Belanghebbende/betrokkende',
      description: "Een belanghebbende is iemand wiens belang bij iets betrokken is; een betrokkene is iemand die zelf bij iets betrokken is."
    },
    {
      word: 'Persona',
      description: "Een persona (of ijkpersoon) is een zeer gedetailleerde omschrijving van een gebruiker van jouw product of dienst. Met behulp van persona's creëer je 'echte' mensen in plaats van algemene doelgroepen die in de praktijk lastig te targeten zijn."
    },
    {
      word: 'Observatie/observeren',
      description: "Observeren is het waarnemen van een persoon en het beschrijven van wat je ziet. Dat kunnen handelingen van bijvoorbeeld kinderen zijn, maar je kunt ook de houding of het gedrag observeren. Observeren in de klas moet zo objectief mogelijk gebeuren. Er is verschil tussen gestructureerd en ongestructureerd observeren."
    },
    {
      word: 'Maquette',
      description: "Model in het klein gebouwd."
    },
    {
      word: 'Requirements',
      description: "Behoefte of eisen waar een product aan voldoet."
    },
    {
      word: 'CE-Markering',
      description: "Veel consumentenproducten die binnen de Europese Unie (EU) op de markt verschijnen, moeten een CE-markering hebben. De CE-markering geeft aan dat het product voldoet aan wettelijke eisen. Denk bijvoorbeeld aan brandveiligheid. Daarnaast is voor veel bouwproducten ook een prestatieverklaring nodig."
    },
    {
      word: 'Mural',
      description: "Een web applicatie voor een soort whiteboard."
    },
    {
      word: 'Gereviseerd',
      description: "Controleren en eventueel corrigeren van onderdelen."
    },
    {
      word: 'Renoveren',
      description: "Opknappen, repareren, vernieuwen, herstellen en zo nodig gedeeltelijk vernieuwen."
    },
    {
      word: 'Definiëren',
      description: "Het helder omschrijven van een kenmerk."
    },
    {
      word: 'Kwantificeren',
      description: "Als meetbare grootheid behandelen. In hoeveelheden uitdrukken of beschouwen."
    },
    {
      word: 'Ecologische',
      description: "Overeenstemming met de natuurlijke verhouding tussen omgeving en de organismen die erin leven."
    },
    {
      word: 'Demografische',
      description: "Een vakgebied waarin de kwantitatieve kenmerken van een bevolking worden bestudeerd."
    },
    {
      word: 'Potentie',
      description: "Beschikbaar vermogen, kracht, macht."
    },
    {
      word: 'Variatie',
      description: "Verschil tussen dingen die verder gelijk zijn."
    },
    {
      word: 'Hufterproof',
      description: "Bestand tegen vandalisme."
    },
    {
      word: 'Waardepropositie',
      description: "Een waardepropositie is een beschrijving van een product of dienst uitgedrukt in de meest waardevolle en onderscheidende elementen in de ogen van een klant."
    },
    {
      word: 'COCD Box',
      description: "Een COCD Box is een selectiemethode om het grote aantal opties uit een divergentie terug te brengen naar een aantal dat je kunt overzien."
    },
  ]

  woordenlijst.sort((a, b) => a.word.localeCompare(b.word));
</script>

<svelte:head>
  <title>Woordenlijst</title>
</svelte:head>

<div>
  <img
    src="images/woordenlijst.jpg"
    alt="woordenlijst"
    width="100%"
    style="height: 400px; object-fit: cover; position: relative;"
  />
  <span
    style="background-color: white; position: absolute; top: 440px; right: 0px;"
    >Foto by <a href="https://unsplash.com/@impatrickt" target="blank"
      >Patrick Tomasso</a
    >
    on <a href="https://unsplash.com/" target="blank">Unsplash</a></span
  >
</div>

<main>
  <div class="left-bar" />
  <div class="content">
    <div class="woordenlijst" id="woordenlijst" style="text-align: justify;">
      <h1>Woordenlijst</h1>

      <div class="woordenlijst-container">
        <div class="woordenlijst-column">
          {#each woordenlijst as word, i}
            {#if i % 2 == 0}
              <p>{word.word}</p>
              <div class="woordenlijst-item">
                <p>
                  {word.description}
                </p>
              </div>
            {/if}
          {/each}
        </div>
        
        <div/>
        <div class="woordenlijst-column">
          {#each woordenlijst as word, i}
            {#if i % 2 == 1}
              <p>{word.word}</p>
              <div class="woordenlijst-item">
                <p>
                  {word.description}
                </p>
              </div>
            {/if}
          {/each}
        </div>
      </div>
    </div>
  </div>
  <div class="right-bar" />
</main>

<style>
  p{
    text-align: left;
  }

  main {
    display: grid;
    grid-template-columns: 25% 50% 25%;
    grid-auto-flow: column;
  }

  .woordenlijst-container {
    display: grid;
    grid-template-columns: 45% 10% 45%;
    margin-bottom: 16px;
  }

  .woordenlijst-container > div {
    margin-bottom: 20px;
  }

  .woordenlijst-item{
    margin-bottom: 1em;
  }

  .woordenlijst-column p {
    margin-top: 0px;
    color: #f06119;
    font-weight: bold;
    margin-bottom: -1px;
  }

  .woordenlijst-item p {
    color: black;
    font-weight: normal;
    margin-top: 0px;
    margin-bottom: 0px;
  }
</style>
