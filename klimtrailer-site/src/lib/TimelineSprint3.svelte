<div class="timeline">
  <div class="spacer" style="height: 100px;"/>
  <div class="container left">
    <div class="content">
      <h2>Ontstaan idee</h2>
      <p>Het ontstaan van de klim wand tijdens meeting met Bosan.</p>
    </div>
  </div>
  <div class="spacer" />
  <div class="container right">
    <div class="content">
      <h2>Prototyping les</h2>
      <p>← Binnen deze les is ons eerste (kartonnen) prototype ontstaan.</p>
    </div>
  </div>
  <div class="spacer" />
  <div class="container left">
    <div class="content">
      <h2>3D prototype</h2>
      <p>Het prototype verder uitwerken in een 3D model en uitprinten.</p>
    </div>
  </div>
  <div class="spacer" />
  <div class="container right">
    <div class="content">
      <h2>Verplaatsbare Boulderwand</h2>
      <p>
        Om het product makkelijker in te zetten binnen meerdere scholen en om zo
        de kosten te drukken hebben we gekozen voor een verplaatsbare versie.
      </p>
    </div>
  </div>
  <div class="spacer" />
  <div class="container left">
    <div class="content">
      <h2>Test dag op Fontys sporthogeschool</h2>
      <p>
        Om ons product hebben we een aantal ALO en Sportkunde docenten gesproken
        over ons idee.
      </p>
    </div>
  </div>
  <div class="spacer" />
  <div class="container right">
    <div class="content">
      <h2>Test met Marc Rompa</h2>
      <p>
        Om ons prototype bij een echte klim specialist te kunnen testen zijn we
        in gesprek gegaan met Marc Rompa.
      </p>
    </div>
  </div>
  <div class="spacer" />
  <div class="container left">
    <div class="content">
      <h2>Iteratie op het 3D model</h2>
      <p>
        Vanuit een onderzoek was gebleken dat de matten dikker zouden moeten
        worden.
      </p>
    </div>
  </div>
  <div class="spacer" />
  <div class="container right">
    <div class="content">
      <h2>Bezoek aan basisschool de kinderboom</h2>
      <p>
        Tijdens dit bezoek hebben we de kans gekregen om met een aantal
        basisschool leerlingen het prototype te testen.
      </p>
    </div>
  </div>
  <div class="spacer" />
  <div class="container left">
    <div class="content">
      <h2>Verschillende wanden</h2>
      <p>
        Om er voor te zorgen dat het product niet saai zal worden voor de
        kinderen zijn er verschillende wanden bedacht doormiddel van een exploratie.
      </p>
    </div>
  </div>
  <div class="spacer" style="height: 350px;"></div>
</div>

<style>
  * {
    box-sizing: border-box;
  }

  .spacer {
    height: 500px;
  }

  /* The actual timeline (the vertical ruler) */
  .timeline {
    position: absolute;
    max-width: 1200px;
    width: 626px;
    margin: 0 auto;
  }

  /* The actual timeline (the vertical ruler) */
  .timeline::after {
    content: "";
    position: absolute;
    width: 6px;
    background-color: gray;
    top: 0;
    bottom: 0;
    left: 50%;
    margin-left: -3px;
  }

  /* Container around content */
  .container {
    padding: 10px 40px;
    position: relative;
    background-color: inherit;
    width: 50%;
  }

  /* The circles on the timeline */
  .container::after {
    content: "";
    position: absolute;
    width: 25px;
    height: 25px;
    right: -17px;
    background-color: white;
    border: 4px solid #004b8e;
    top: 15px;
    border-radius: 50%;
    z-index: 1;
  }

  /* Place the container to the left */
  .left {
    left: 0;
  }

  /* Place the container to the right */
  .right {
    left: 50%;
  }

  /* Add arrows to the left container (pointing right) */
  .left::before {
    content: " ";
    height: 0;
    position: absolute;
    top: 22px;
    width: 0;
    z-index: 1;
    right: 30px;
    border: medium solid white;
    border-width: 10px 0 10px 10px;
    border-color: transparent transparent transparent white;
  }

  /* Add arrows to the right container (pointing left) */
  .right::before {
    content: " ";
    height: 0;
    position: absolute;
    top: 22px;
    width: 0;
    z-index: 1;
    left: 30px;
    border: medium solid white;
    border-width: 10px 10px 10px 0;
    border-color: transparent white transparent transparent;
  }

  /* Fix the circle for containers on the right side */
  .right::after {
    left: -16px;
  }

  /* The actual content */
  .content {
    padding: 20px 30px;
    background-color: white;
    position: relative;
    border-radius: 6px;
  }

  /* Media queries - Responsive timeline on screens less than 600px wide */
  @media screen and (max-width: 600px) {
    /* Place the timelime to the left */
    .timeline::after {
      left: 31px;
    }

    /* Full-width containers */
    .container {
      width: 100%;
      padding-left: 70px;
      padding-right: 25px;
    }

    /* Make sure that all arrows are pointing leftwards */
    .container::before {
      left: 60px;
      border: medium solid white;
      border-width: 10px 10px 10px 0;
      border-color: transparent white transparent transparent;
    }

    /* Make sure all circles are at the same spot */
    .left::after,
    .right::after {
      left: 15px;
    }

    /* Make all right containers behave like the left ones */
    .right {
      left: 0%;
    }
  }
</style>
