<svelte:head>
  <title>Bosan Portfolio</title>
</svelte:head>

<div class="title_screen">

  <ul class="nav homepage">
    <a class="navbar-brand" href="index.svelte">
      <img src="logo.jpg" alt="Logo" width="30px"/>
    </a>
    <li><a href="">Opdracht</a></li>
  </ul>

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

<div style="margin-top: 1000px;">
  <p>testdsfdsfdsfsd sdfdsfdsf sdfdsfsd sdfdsfsdf</p>
</div>

<style>
  .title_screen {
    width: 100%;
    height: 1px;
    position: relative;
  }

  .homepage {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
  }

  .homepage > * {
    margin: 0 0;
  }

  .nav {
    list-style-type: none;
    top: -16px;
    padding: 0;
    z-index: 1;
  }

  .nav > a > img {
    padding: 14px;
  }

  .nav > li {
    float: right;
    font-size: 18pt;
  }

  .nav > li > a {
    display: block;
    text-align: center;
    padding: 14px;
    text-decoration: none;
  }

  .nav > li > a:hover {
    background-color: #004B8E;
    color: white;

    -webkit-transition-duration: 200ms; /* Vertraag het hoveren */
    transition-duration: 200ms;
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
    width: 100vw;
    height: 100vh;
    background-color: white;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
  }

  .div_two {
    width: 100vw;
    height: 100vh;
    background-image: url("klimtrailer6.png");
    clip-path: polygon(58vw 0, 0% 280vh, 1000000vw 100vh);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
  }
</style>
