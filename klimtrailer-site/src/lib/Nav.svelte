<script>
  import { goto } from "$app/navigation";

  export let pagePath = undefined;

  let showDropdown = false;

  function onNavDropdownClick(){
    showDropdown = !showDropdown;
  }
</script>

<ul class="nav {pagePath == '/' ? 'homepage' : 'normalpage'}">
  <a class="navbar-brand" href="/">
    <img src="images/logo.png" alt="Logo" width="30px" />
  </a>
  <!-- svelte-ignore a11y-missing-attribute -->
  <li on:click={onNavDropdownClick}><a>Sprints <i class="fa-solid fa-angle-down"></i></a></li>
  <li><a href="gegevens">Gegevens</a></li>
  <li><a href="woordenlijst">Woordenlijst</a></li>
  <li><a href="bronvermelding">Bronvermelding</a></li>
</ul>

{#if showDropdown}
    <div class="nav-dropdown-backdrop" on:click={onNavDropdownClick}></div>
    <div class="nav-dropdown-menu" on:click={onNavDropdownClick} style="{pagePath == '/' ? 'margin-top: 69px;' : 'margin-top: 5px;'}">
      <ul>
        <li on:click={() => {goto('/sprint1')}}><a href="sprint1">Sprint 1: Analyse</a></li>
        <li on:click={() => {goto('/sprint2')}}><a href="sprint2">Sprint 2: Brainstorms</a></li>
        <li on:click={() => {goto('/sprint3')}}><a href="sprint3">Sprint 3: Prototyping</a></li>
        <li on:click={() => {goto('/sprint4')}}><a href="sprint4">Sprint 4: Usertesting</a></li>
        <li on:click={() => {goto('/sprint5')}}><a href="sprint5">Sprint 5: Demo Day Lite</a></li>
        <li on:click={() => {goto('/sprint6')}}><a href="sprint6">Sprint 6: Afronding</a></li>
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
