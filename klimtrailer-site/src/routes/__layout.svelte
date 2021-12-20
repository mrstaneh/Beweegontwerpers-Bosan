<ul class="nav homepage">
  <a class="navbar-brand" href="index.svelte">
    <img src="logo.jpg" alt="Logo" width="30px" />
  </a>
  <li><a href="">Opdracht</a></li>
</ul>
<slot />

<style>
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
    background-color: #004b8e;
    color: white;

    -webkit-transition-duration: 200ms; /* Vertraag het hoveren */
    transition-duration: 200ms;
  }
</style>
