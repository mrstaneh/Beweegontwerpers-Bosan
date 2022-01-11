<script>
  export let pagePath = undefined;
</script>

<ul class="nav {pagePath == '/' ? 'homepage' : 'normalpage'}">
  <a class="navbar-brand" href="/">
    <img src="images/logo.png" alt="Logo" width="30px" />
  </a>
  <li><a href="gegevens">Gegevens</a></li>
  <li><a href="woordenlijst">Woordenlijst</a></li>
  <li><a href="bronvermelding">Bronvermelding</a></li>
</ul>

<style>
  .homepage {
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
  }

  .normalpage {
    margin: 0;
    background-color: white;
    /* background-color: #b2b2b2; */
  }

  .homepage > * {
    margin: 0 0;
  }

  .nav {
    list-style-type: none;
    top: -16px;
    padding: 0;
    z-index: 1;
    height: 64px;
  }

  .nav > a > img {
    padding: 16px 14px 14px 14px;
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
    background-color: #004b8e;
    color: white;

    -webkit-transition-duration: 200ms; /* Vertraag het hoveren */
    transition-duration: 200ms;
  }
</style>
