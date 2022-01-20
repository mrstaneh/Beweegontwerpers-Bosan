<script>
  import { goto } from "$app/navigation";

  export let pagePath = undefined;

  let showDropdown = false;

  function onNavDropdownClick(){
    showDropdown = !showDropdown;
  }
</script>

<ul class="nav {pagePath == '/' ? 'homepage' : 'normalpage'}">
  <div class="navbar-logo">
    <img src="images/logo.png" alt="Logo" width="40px" height="40px" on:click={() => {goto('/')}}/>
    <a href="/">Portfolio</a>
  </div>
  <!-- svelte-ignore a11y-missing-attribute -->
  <li on:click={onNavDropdownClick}><a>Inhoud <i class="fa-solid fa-angle-down"></i></a></li>
  <li><a href="contact">Contact</a></li>
  <li><a href="woordenlijst">Woordenlijst</a></li>
  <li><a href="bronvermelding">Bronvermelding</a></li>
  <li><a href="bijlagen">Bijlagen</a></li>
</ul>

{#if showDropdown}
    <div class="nav-dropdown-backdrop" on:click={onNavDropdownClick}></div>
    <div class="nav-dropdown-menu" on:click={onNavDropdownClick} style="{pagePath == '/' ? 'margin-top: 69px;' : 'margin-top: 5px;'}">
      <ul>
        <li on:click={() => {goto('/proces')}}><a href="proces">Proces</a></li>
        <li on:click={() => {goto('/brainstorms')}}><a href="brainstorms">Brainstorms</a></li>
        <li on:click={() => {goto('/usertesting')}}><a href="usertesting">Usertesting</a></li>
        <li on:click={() => {goto('/personas')}}><a href="personas">Persona's</a></li>
        <li on:click={() => {goto('/wetgevingen')}}><a href="personas">Wetgevingen</a></li>
        <li on:click={() => {goto('/businessmodel')}}><a href="businessmodel">Business Model Canvas</a></li>
        <li on:click={() => {goto('/demodaylite')}}><a href="demodaylite">Demo Day Lite</a></li>
        <li on:click={() => {goto('/mixandmatch')}}><a href="mixandmatch">Mix and Match</a></li>
        <li on:click={() => {goto('/afronding')}}><a href="afronding">Afronding</a></li>
      </ul>
    </div>
{/if}


<style>
  .homepage {
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
  }

  .navbar-logo{
    display: inline;
  }

  .navbar-logo img{
    margin-left: 11px;
    padding-top: 11px;
  }

  .navbar-logo img:hover{
    cursor: pointer;
  }

  .navbar-logo a{
    position: relative;
    left: 10px;
    top: -6px;
    font-size: 36px;
  }

  .nav-dropdown-backdrop{
    position: fixed;
    top: 64px;
    height: calc(100% - 64px);
    width: 100%;
    z-index: 998;
  }

  .nav-dropdown-menu{
    position: fixed;
    display: flex;
    flex-direction: column;
    background-color: white;
    box-shadow: 0 2px 4px 0 rgba(0, 0, 0, .2);
    border: 1px solid #4A4A55;
    right: 5px;
    z-index: 999;
  }

  .nav-dropdown-menu ul{
    margin-block-start: 0px;
    margin-block-end: 0px;
    padding-inline-start: 00px;
    padding-inline-end: 00px;
    list-style: none;
  }

  .nav-dropdown-menu ul li{
    padding: 6px;
    padding-left: 20px;
    padding-right: 20px;
    cursor: pointer;
  }

  .nav-dropdown-menu ul li:hover{
    background-color: rgb(235, 235, 235);
  }

  .nav-dropdown-menu ul li a{
    font-size: 24px;
  }

  .normalpage {
    margin: 0;
    background-color: white;
    /* background-color: #b2b2b2; */
  }

  .homepage > * {
    margin: 0 0;
  }

  a:hover{
    cursor: pointer;
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
