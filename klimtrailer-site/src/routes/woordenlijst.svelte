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
          <p>Primair Onderwijs</p>
          <div class="woordenlijst-item">
            <p>
              Primair onderwijs is de overkoepelende sector voor het
              basisonderwijs én het speciaal basisonderwijs (SBO)
            </p>
          </div>
        </div>
        <div/>
        <div class="woordenlijst-column">
          <p>Stakeholder</p>
          <div class="woordenlijst-item">
            <p>
              Stakeholders zijn personen of groepen van personen die een direct
              of indirect belang hebben bij de organisatie en/of omgekeerd.
              Kortom alle belanghebbenden.
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

  .woordenlijst-container {
    display: grid;
    grid-template-columns: 45% 10% 45%;
    margin-bottom: 16px;
  }

  .woordenlijst-container > div {
    margin-bottom: 20px;
  }

  .woordenlijst-column p {
    margin-top: 0px;
    color: #f06119;
    font-weight: bold;
    margin-bottom: 4px;
  }

  .woordenlijst-item p {
    color: black;
    font-weight: normal;
    margin-top: 0px;
    margin-bottom: 0px;
  }
</style>
