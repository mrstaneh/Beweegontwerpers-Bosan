<script>
  import { onMount } from "svelte";

  let bronnen = [
    {
      text: "1 Moscow methode",
      url: "pdf-bijlage/moscow.pdf",
    },
    {
      text: "2 Interviews",
      url: "pdf-bijlage/interviews.pdf",
      
    },
    {
      text: "3 Cimo's",
      url: "pdf-bijlage/cimos.pdf",
    },
    {
      text: "4 Prototype",
      url: "pdf-bijlage/prototype.pdf",
    },
    {
      text: "5 Prototype testen",
      url: "pdf-bijlage/prototype-test.pdf",
    },
    {
      text: "6 Massa en afmeting berekening (Mini Boulder)",
      url: "pdf-bijlage/Massa-en-afmetingen.pdf",
    },
    {
      text: "7 Link naar alle murals",
      url: "pdf-bijlage/murals.pdf",
    },
  ];

  onMount(() => {
    let element = document.getElementById(
      window.location.hash.replace("#", "")
    );

    if (element) {
      element.style.backgroundColor = "#ccd7ff";
    }
  });
</script>

<svelte:head>
  <title>Bijlagen</title>
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
    <div class="bijlagen" id="bijlagen" style="text-align: justify;">
      <h1>Bijlagen</h1>

      <div class="bijlagen-container">
        <div class="bijlagen-column">
          {#each bronnen as bron, i}
            {#if 1}
              <div class="bijlagen-item">
                <p id={i + 1}>
                  {bron.text + ": "}<a target="_blank" href={bron.url}>link</a>
                </p>
              </div>
            {/if}
          {/each}
        </div>
        <div class="bijlagen-column" />
      </div>
    </div>
  </div>
  <div class="right-bar" />
</main>

<style>
  p {
    text-align: left;
  }

  main {
    display: grid;
    grid-template-columns: 25% 50% 25%;
    grid-auto-flow: column;
  }

  .bijlagen-column {
    display: grid;
    grid-template-columns: 45% 45%;
    column-gap: 10%;
  }

  .bijlagen-container > div {
    margin-bottom: 20px;
  }

  .bijlagen-column p {
    margin-top: 0px;
    color: #f06119;
    font-weight: bold;
    margin-bottom: 4px;
  }

  .bijlagen-item {
    overflow-x: hidden;
    margin-bottom: 1em;
  }

  .bijlagen-item p {
    border-radius: 4px;
    padding: 4px;
    color: black;
    font-weight: normal;
    margin-top: 0px;
    margin-bottom: 0px;
  }
</style>
