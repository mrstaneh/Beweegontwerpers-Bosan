<script>
  import { onMount } from 'svelte';

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
          <div class="bronnenlijst-item">
            <p id="1">
              [1] Van der Meer, P. (2020, 5 februari). Twee uur gym wordt
              verplicht in primair onderwijs. Geraadpleegd op 6 oktober 2021,
              van <a
                target="_blank"
                href="https://www.sportenstrategie.nl/overheid/twee-uur-gym-wordt-verplicht-in-primair-onderwijs/"
                >https://www.sportenstrategie.nl/overheid/twee-uur-gym-wordt-verplicht-in-primair-onderwijs/</a
              >
            </p>
          </div>
        </div>
        <div />
        <div class="bronnenlijst-column">
          <div class="bronnenlijst-item">
            <p id="2">
              [2] Sport & Gemeenten. (2020, 7 februari). Vereniging Sport en
              Gemeenten » Twee uur gym verplicht op basisschool. Geraadpleegd op
              6 oktober 2021, van <a
                target="_blank"
                href="https://sportengemeenten.nl/twee-uur-gym-verplicht-op-basisschool/"
                >https://sportengemeenten.nl/twee-uur-gym-verplicht-op-basisschool/
              </a>
            </p>
          </div>
        </div>
        <div class="bronnenlijst-column">
          <div class="bronnenlijst-item">
            <p id="3">
              [3] Romijn, D., & Schadenberg, B. (2019 februari). Ruimte voor
              binnensport in Tilburg. Geraadpleegd op 6 oktober 2021, van <a
                target="_blank"
                href="https://www.kennisbanksportenbewegen.nl/?file=9452&m=1554388827&action=file.download"
                >https://www.kennisbanksportenbewegen.nl/?file=9452&m=1554388827&action=file.download
              </a>
            </p>
          </div>
        </div>
        <div />
        <div class="bronnenlijst-column">
          <div class="bronnenlijst-item">
            <p id="4">
              [4] Brouwer, L., Slot-Heijs, J., Lucassen, J., & Collard, D. (2018
              december). Veiligheid in het bewegingsonderwijs. Geraadpleegd op 6
              oktober 2021, van <a
                target="_blank"
                href="https://www.kennisbanksportenbewegen.nl/?file=8996&m=1533214923&action=file.download"
                >https://www.kennisbanksportenbewegen.nl/?file=8996&m=1533214923&action=file.download
              </a>
            </p>
          </div>
        </div>
        <div class="bronnenlijst-column">
          <div class="bronnenlijst-item">
            <p id="5">
              [5] CIOS. (2020, 7 februari). Minimaal 2 uur gym op school | CIOS.
              Geraadpleegd op 3 november 2021, van <a
                target="_blank"
                href="https://www.cios.nl/nieuws/minimaal-2-uur-gym-op-school"
                >https://www.cios.nl/nieuws/minimaal-2-uur-gym-op-school
              </a>
            </p>
          </div>
        </div>
        <div />
        <div class="bronnenlijst-column">
          <div class="bronnenlijst-item">
            <p id="6">
              [6] Ministerie van Volksgezondheid, Welzijn en Sport. (2021, 10
              maart). Sporten en bewegen voor kinderen. Sport en bewegen |
              Rijksoverheid.nl. Geraadpleegd op 1 december 2021, van <a
                target="_blank"
                href="https://www.rijksoverheid.nl/onderwerpen/sport-en-bewegen/sporten-en-bewegen-voor-kinderen"
                >https://www.rijksoverheid.nl/onderwerpen/sport-en-bewegen/sporten-en-bewegen-voor-kinderen
              </a>
            </p>
          </div>
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

  .bronnenlijst-container {
    display: grid;
    grid-template-columns: 45% 10% 45%;
    margin-bottom: 16px;
  }

  .bronnenlijst-container > div {
    margin-bottom: 20px;
  }

  .bronnenlijst-column p {
    margin-top: 0px;
    color: #f06119;
    font-weight: bold;
    margin-bottom: 4px;
  }

  .bronnenlijst-item p {
    color: black;
    font-weight: normal;
    margin-top: 0px;
    margin-bottom: 0px;
  }
</style>
