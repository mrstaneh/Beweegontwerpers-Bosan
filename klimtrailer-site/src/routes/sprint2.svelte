<script>
  import InhoudItem from "$lib/InhoudItem.svelte";
  import TimelineSprint1 from "$lib/TimelineSprint1.svelte";
</script>

<svelte:head>
  <title>Sprint 2</title>
</svelte:head>

<main>
  <div class="left-bar" />
  <div class="content">
    <h1>Sprint 2: Brainstorms</h1>
    <div class="section brainstorm" id="brainstorm">
      <h1>Brainstorm</h1>
      <iframe
        title="Mural"
        src="https://app.mural.co/embed/2551f8da-bf76-45d8-874a-3ae60cb5103a"
        width="100%"
        height="480px"
        style="min-width: 640px; min-height: 480px; background-color: #f4f4f4; border: 1px solid #efefef"
        sandbox="allow-same-origin allow-scripts allow-modals allow-popups allow-popups-to-escape-sandbox"
      />
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
