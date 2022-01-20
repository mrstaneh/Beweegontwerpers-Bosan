<script>
    import Mural from "$lib/Mural.svelte";
</script>

<svelte:head>
  <title>Business Model Canvas</title>
</svelte:head>
<main>
  <div class="left-bar" />
  <div class="content">
    <h1>Business Model Canvas</h1>
    <div class="section businessmodelcanvas" id="businessmodelcanvas">
      <h1 style="margin-right: 6px; margin-bottom: 0px;">Business Model Canvas</h1>
      <p style="color: #F06119; display: inline;">Hoe werkt het BMC?</p>
      <p>Het doel van een Business model canvas is inzicht krijgen in wat er allemaal komt kijken bij een bedrijfsvoering. Het is verstandig om hier van tevoren over na te denken, dit is de ruggengraat van het bedrijf en bepaald of het levensvatbaar is. Dit is een model wat regelmatig geüpdatet moet worden, vanwege een constant veranderende markt. </p>
      <p>Alle kanalen zijn belangrijk in dit model, als er één wordt overslagen kan dit fatale gevolgen hebben voor een bedrijf. 
        De key resources en key partners zijn hierbij van groot belang, door dit van tevoren goed in de gaten kunnen mogelijke tegenslagen worden voorkomen. Elk startend maar ook elk bestaand bedrijf zou dus veel waarde moeten hechten aan het BMC.          
        </p>

      <p style="color: #F06119; display: inline;">Hoe is een BMC opgebouwd?</p>
      <p>Er wordt gestart met een klant profiel en een value map. Deze zijn opgedeeld in pijn, voordelen en taken voor de klant. De value map bestaat uit producten, pijnverzachters en voordelen. Nadat deze duidelijk zijn kan het volledige Business Model Canvas worden ingevuld. </p>
      <p>Bij het BMC is het ook van belang dat er een juiste volgorde wordt gehanteerd. Deze is als volgt:</p>
      <ol>
        <li>Klantsegmenten</li>
        <li>Waardepropositie</li>
        <li>Klantrelaties</li>
        <li>Kanalen</li>
        <li>Inkomstenstromen</li>
        <li>Hulpbronnen</li>
        <li>Partners</li>
        <li>Kostenstructuur</li>
      </ol>
      <p>Onder in het BMC model zijn de belangrijkste pijlers te zien, dit zijn de inkomensstromen en de kostenstructuur. Deze bepalen uiteindelijk de mogelijke omzet voor het bedrijf en geeft dus antwoord op de vraag of het bedrijf levensvatbaar zal zijn.</p>

      <p style="color: #F06119; display: inline;">Toelichting van het BMC</p>
      <p>Allereerst is er door iedereen apart nagedacht over het klantenprofiel en de value map, vervolgens is dit besproken en samengevoegd tot één geheel. Hier zijn verschillende pijnpunten bij naar voren gekomen, een belangrijke is de veiligheid en de verkoopprijs in aanschaf. Een bijpassende pijnverzachter hiervoor is een goede valmat en een valinstructie.</p>
      <p>Bij de kostenstructuur is gekeken naar de materiaalkosten, marketingkosten, variabele kosten en de vaste kosten. Ook zijn de afschrijvingen meegenomen en is er nagedacht over eventueel gebruik van massaproductie. Dit zijn de belangrijkste punten die naar voren kwamen uit het BMC.</p>

      <p style="color: #F06119; display: inline;">Conclusie</p>
      <p>De veranderende markt speelt voor Bosan vooral bij de materiaalkosten. Deze kosten zullen in de toekomst toenemen, dit zal invloed hebben op de markt maar ook op het BMC. 
        [<a target="_blank" href="bronvermelding/#12">12</a>] 
        Deze prijs zal constant veranderen wat resulteert in een constant veranderend BMC.</p>

      <Mural title="BMC" src="https://app.mural.co/embed/b43356ae-b9de-4ecd-9a3a-50f00b649976"/>
    </div>
    <a style="margin-bottom: 20px;" href="demodaylite" class="button"
      >Ga naar de volgende pagina</a
    >
  </div>
  <div class="right-bar" />
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

  p {
    margin-top: 0;
  }
</style>
