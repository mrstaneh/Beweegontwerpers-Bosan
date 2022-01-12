<svelte:head>
  <title>Bosan Portfolio</title>
</svelte:head>

<div class="title_screen">

  <div class="div_one homepage" />
  <div class="div_two homepage" />
  <div class="overlay homepage" />
  <div class="box homepage">
    <h2 style="color: #004B8E; font-size: 40px;">Team Bosan</h2>
    <h1 style="font-size: 165px; margin: -70px -10px;">Portfolio</h1>
    <h3 style="font-size: 40px;">Minor beweegontwerper</h3>
    <br />
    <br>
    <p style="display: inline; font-size: 25px;">
      Op deze site zal u het proces terug vinden van de
      <span style="color: #004B8E; display: inline;">"Boulder Mini"</span>
      . Er zal verteld worden waaruit het idee ontstaan is, hoe dit onderbouwd is
      en hoe we het probleem willen aanpakken.
    </p>
  </div>
  <div class="arrow homepage" />
</div>

<style>
  .title_screen {
    width: 1900px;
    height: 1080px;
    position: relative;
  }

  .homepage {
    width: 1900px;
    height: 1080px;
    position: absolute;
    top: 0;
    left: 0;
  }

  .homepage > * {
    margin: 0 0;
  }

  .box {
    width: 30%;
    left: 5%;
    margin-top: 10%;
  }

  .box > * {
    color: black;
  }

  .div_one {
    width: 1900px;
    height: 1080px;
    background-color: white;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
  }

  .div_two {
    width: 1900px;
    height: 1080px;
    background-image: url("/images/klimtrailer6.png");
    clip-path: polygon(58vw 0, 0% 280vh, 1000000vw 100vh);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
  }
</style>
