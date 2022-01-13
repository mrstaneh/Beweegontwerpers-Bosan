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
      <p>We zijn begonnen met idee frames uit te werken. Hierbij was de eerste stap een naam verzinnen van het idee. Vervolgens ga je het idee beschrijven en dit koppelen aan een waarde propositie. Onderaan het frame wordt het probleem kernachtig neer gezet en al meteen gekeken naar een oplossingsrichting. Hierbij ga je ook meteen breed kijken naar alternatieven. Het is van belang dat de idee frames niet vast staan vanaf het begin. Hier kan gedurende het ontwerp proces een evolutie in plaats vinden. Zo komt het ook voor dat sommige frames op elkaar lijken. Deze zijn dan samengevoegd naar een frame
        . Bij het begin frame is er gekeken naar minimaal 2 uur gym en het frame daarna ‘buiten gymmen’. Deze lijken in essentie veel op elkaar. Vandaar dat deze zijn samengevoegd.
        </p>
      <p>Het is ook mooi als een frame visueel is. Door gebruik te maken van een schets kan het frame veel vertellen over de inhoud. 
        Je gaat dus eigenlijk breed kijken naar een oplossing richting voor een probleem. 
        </p>
        <iframe title="Frames" src='https://app.mural.co/embed/27e91e81-af67-4650-ae4c-dc59a218d101'
        width='100%'
        height='480px'
        style='min-width: 640px; min-height: 480px; background-color: #f4f4f4; border: 1px solid #efefef'
        sandbox='allow-same-origin allow-scripts allow-modals allow-popups allow-popups-to-escape-sandbox'>
        </iframe>
    </div>
    <div class="section cimo" id="cimo">
      <h1>CIMO Analyses</h1>
      <p>Een CIMO analyse bestaat uit 4 delen zoals afgebeeld in de foto hier onder.</p>
      <img style="width: 60%;" src="/images/cimo.jpg" alt="CIMO"/>
      <p>Vanaf sprint 2 hebben we voor iedere sprint deze analyse ingevuld. Hierdoor hebben wij ons doel per sprint beter voor ogen en hebben we al nagedacht over de stappen die we moeten doorlopen om ons doel te halen. Hieronder staat de mural waar al onze CIMOs van het project staan.</p>
      <iframe title="CIMOs" src='https://app.mural.co/embed/b00af80c-18cd-4182-8a31-160205b9a1eb'
        width='100%'
        height='480px'
        style='min-width: 640px; min-height: 480px; background-color: #f4f4f4; border: 1px solid #efefef'
        sandbox='allow-same-origin allow-scripts allow-modals allow-popups allow-popups-to-escape-sandbox'>
      </iframe>
    </div>
  </div>
  <div class="right-bar">
    <TimelineSprint1 />
  </div>
</main>
