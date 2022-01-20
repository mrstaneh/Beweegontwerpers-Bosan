<script>
  import { onMount } from 'svelte';

  let bronnen = [
    {
      text: '[1] Van der Meer, P. (2020, 5 februari). Twee uur gym wordt verplicht in primair onderwijs. Geraadpleegd op 6 oktober 2021, van ',
      url: 'https://www.sportenstrategie.nl/overheid/twee-uur-gym-wordt-verplicht-in-primair-onderwijs/'
    },
    {
      text: '[2] Sport & Gemeenten. (2020, 7 februari). Vereniging Sport en Gemeenten » Twee uur gym verplicht op basisschool. Geraadpleegd op 6 oktober 2021, van ',
      url: 'https://sportengemeenten.nl/twee-uur-gym-verplicht-op-basisschool/'
    },
    {
      text: '[3] Romijn, D., & Schadenberg, B. (2019 februari). Ruimte voor binnensport in Tilburg. Geraadpleegd op 6 oktober 2021, van ',
      url: 'https://www.kennisbanksportenbewegen.nl/?file=9452&m=1554388827&action=file.download'
    },
    {
      text: '[4] Brouwer, L., Slot-Heijs, J., Lucassen, J., & Collard, D. (2018 december). Veiligheid in het bewegingsonderwijs. Geraadpleegd op 6 oktober 2021, van',
      url: 'https://www.kennisbanksportenbewegen.nl/?file=8996&m=1533214923&action=file.download'
    },
    {
      text: '[5] CIOS. (2020, 7 februari). Minimaal 2 uur gym op school | CIOS. Geraadpleegd op 3 november 2021, van ',
      url: 'https://www.cios.nl/nieuws/minimaal-2-uur-gym-op-school'
    },
    {
      text: '[6] Ministerie van Volksgezondheid, Welzijn en Sport. (2021, 10 maart). Sporten en bewegen voor kinderen. Sport en bewegen | Rijksoverheid.nl. Geraadpleegd op 1 december 2021, van ',
      url: 'https://www.rijksoverheid.nl/onderwerpen/sport-en-bewegen/sporten-en-bewegen-voor-kinderen'
    },
    {
      text: '[7] Awasthi, B & Conrad, A (2021 March).  Research Online, Purchase Offline: Why Are Customers Driven to the Omnichannel Experience? Geraadpleegd op 22 december 2021, van ',
      url: 'https://www.getapp.com/resources/research-online-purchase-offline-omnichannel/'
    },
    {
      text: '[8] NKBV. (z.d.). NORMERING/KEURING VAN KLIMWANDEN. Geraadpleegd op 13 januari 2022, van ',
      url: 'https://nkbv.nl/kenniscentrum/normering-keuring-van-klimwanden.html'
    },
    {
      text: '[9] Cleanbing, nieuw in het assortiment. (z.d.). KLIMWANDSERVICE. Geraadpleegd op 13 januari 2022, van ',
      url: 'https://kl[i]mwandenservice.nl/2017/11/07/cleanbing-nieuw-i'
    },
    {
      text: '[10] kenniscentrum sportklimmen (2010, maart). Geraadpleegd op 12 januari 2022 van ',
      url: 'https://nkbv.nl/files/Kenniscentrum/Sportklimmen/HL_3-2010_p60-63_Spot_me.pdf'
    },
    {
      text: '[11] Buitenspelen in de wijk krijgt een boost(2021, juni). Geraadpleegd op 10 januari 2022 van ',
      url: 'https://www.allesoversport.nl/thema/beweegstimulering/buitenspelen-in-de-wijk-krijgt-een-boost-met-de-pop-upspeelplek/'
    },
    {
      text: '[12] Peter de Waard. De Volkskrant. (maart 2021). Grondstofprijzen exploderen en dat kan voor veel mkb-bedrijven het einde betekenen. Geraadpleegd januari 2022 van ',
      url: 'https://www.volkskrant.nl/kijkverder/tracken-trace/v/een-wc-papiertje-of-kopje-koffie-is-door-prijsexplosie-grondstoffen-plots-veel-duurder/'
    },
    {
      text: '[13] Volksgezondheidenzorg. (z.d.). Sport op de kaart | Aanbod | Sportaccommodaties | Volksgezondheidenzorg.info. Geraadpleegd op 28 september 2021, van ',
      url: 'https://www.volksgezondheidenzorg.info/sport/sportopdekaart/sportaccommodaties#node-sporthallen-gemeente'
    },
    {
      text: '[14] Schadenberg, B., & Romijn, D. (2019, februari). Ruimte voor binnensport in Tilburg. Mulier instituut. Geraadpleegd op 28 september 2021, van ',
      url: 'https://www.kennisbanksportenbewegen.nl/?file=9452&m=1554388827&action=file.download'
    },
    {
      text: '[15] Homan, C. (2017, 13 mei). KNMI - Hevigere buien door klimaatverandering. knmi. Geraadpleegd op 28 september 2021, van ',
      url: 'https://www.knmi.nl/over-het-knmi/nieuws/hevigere-buien-door-klimaatverandering'
    },
    {
      text: '[16] Visser, K., Tiessen-Raaphorst, A., Van Bakel, M., & De Vries, M. (2016, mei). Sport Toekomst Verkenning. sportenbewegenincijfers. Geraadpleegd op 29 september 2021, van ',
      url: 'https://www.sportenbewegenincijfers.nl/sites/default/files/2017-06/20160519%20Sport%20Toekomstverkenning%20drijvende%20krachten%20sport%20en%20bewegen.pdf '
    },
    {
      text: '[17] Ensberg-Kleijkers, D. (2019, mei). Jantje Beton. Geraadpleegd op 29 september 2021, van ',
      url: 'https://jantjebeton.nl/uploads/downloads/onderzoek-buitenspelen-2019-5cffc1bd70afd.pdf'
    },
  ]

  onMount(() => {
    let element = document.getElementById(window.location.hash.replace('#', ''));

    if(element){
      element.style.backgroundColor = '#ccd7ff';
    }
  });
</script>

<svelte:head>
  <title>Bronvermelding</title>
</svelte:head>

<div>
    <img
      src="images/bronvermeling.jpg"
      alt="woordenlijst"
      width="100%"
      style="height: 400px; object-fit: cover; position: relative;"
    />
    <span
      style="background-color: white; position: absolute; top: 440px; right: 0px;"
      >Foto by <a href="https://unsplash.com/@homajob" target="blank"
        >Scott Graham</a
      >
      on <a href="https://unsplash.com/" target="blank">Unsplash</a></span
    >
</div>

<main>
  <div class="left-bar" />
  <div class="content">
    <div class="bronnenlijst" id="bronnenlijst" style="text-align: justify;">
      <h1>Bronnenlijst</h1>

      <div class="bronnenlijst-container">
        <div class="bronnenlijst-column">
          {#each bronnen as bron, i}
              <div class="bronnenlijst-item">
                <p id="{i+1}">
                  {bron.text}<a
                    target="_blank"
                    href="{bron.url}"
                    >{bron.url}</a
                  >
                </p>
              </div>
          {/each}
        </div>
        <div class="bronnenlijst-column">
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
  .bronnenlijst-container > div {
    margin-bottom: 20px;
  }

  .bronnenlijst-column {
    display: grid;
    grid-template-columns: 45% 45%;
    column-gap: 10%;
  }

  .bronnenlijst-column p {
    margin-top: 0px;
    color: #f06119;
    font-weight: bold;
    margin-bottom: 4px;
  }

  .bronnenlijst-item{
    overflow-x: hidden;
    margin-bottom: 1em;
    height: 160px;
  }

  .bronnenlijst-item p {
    border-radius: 4px;
    padding: 4px;
    color: black;
    font-weight: normal;
    margin-top: 0px;
    margin-bottom: 0px;
  }
</style>
