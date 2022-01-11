<script>
  import InhoudItem from "$lib/InhoudItem.svelte";
  import TimelineSprint1 from "$lib/TimelineSprint1.svelte";
</script>

<svelte:head>
  <title>Sprint 4</title>
</svelte:head>

<main>
  <div class="left-bar" />
  <div class="content">
    <h1>Sprint 4: Usertesting</h1>
    <div class="section brainstorm" id="brainstorm">
      <h1>Brainstorm</h1>
    </div>
    <div class="section frames" id="frames">
      <h1>Frames</h1>
    </div>
    <div class="section prototyping" id="prototyping">
      <h1>Prototyping</h1>
    </div>
    <div class="section proces" id="proces">
      <h1>Proces</h1>
    </div>
  </div>
  <div class="right-bar">
    <TimelineSprint1 />
  </div>
</main>
