<div class="timeline">
  <div class="spacer" />
  <div class="container left">
    <div class="content">
      <h2>Introductie CIMO analyse</h2>
      <p>
        ← Om een doel aan onze sprints te geven hebben we gebruik gemaakt van
        CIMO's.
      </p>
    </div>
  </div>
  <div class="spacer" style="height: 350px;" />
  <div class="container right">
    <div class="content">
      <h2>Bedenken van de brainstorm vraag</h2>
      <p>
        Met deze vraag zijn we later gaan brainstomen om op ons idee te komen.
      </p>
    </div>
  </div>
  <div class="spacer" style="height: 150px;" />
  <div class="container left">
    <div class="content">
      <h2>Brainstormen</h2>
      <p>
        ← Meerder creatieve sessies voor ons idee, zoals: Teleportstroming,
        Sketching, etc.
      </p>
    </div>
  </div>
  <div class="spacer" />
  <div class="container right">
    <div class="content">
      <h2>Empathy map</h2>
      <p><a href="https://app.mural.co/t/beweegontwerper5597/m/beweegontwerper5597/1634542681046/b35741fd117129d7b49ca45462004a8abcfa8093?sender=uda85e330004642c3ab2b4218" target="_blank">link</a></p>
    </div>
  </div>
  <div class="spacer" />
  <div class="container left">
    <div class="content">
      <h2>Frames</h2>
      <p>
        ← Om ons project vanuit meerdere hoeken hebben we gebruik gemaakt van
        frames.
      </p>
    </div>
  </div>
  <div class="spacer" style="height: 550px;" />
</div>

<style>
  * {
    box-sizing: border-box;
  }

  .spacer {
    height: 100px;
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
