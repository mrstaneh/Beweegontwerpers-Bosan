<div class="timeline">
  <div class="container left">
    <div class="content">
      <h2>Start persona's</h2>
      <p>Het begin van onze persona's.</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h2>Een nieuw gymtoestel</h2>
      <p>Casper, Rafaël en Nicky.</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h2>Een verplaatsbaar toestel</h2>
      <p>Luca.</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h2>Creatief te gebruiken</h2>
      <p>Joris.</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h2>Aantal mensen tegelijk op het toestel</h2>
      <p>Mariec en Marc.</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h2>Verschillende boulder niveaus mogelijk</h2>
      <p>Luca, Mariec, Casper, Rafaël en Nicky.</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h2>Verlichting in de grepen</h2>
      <p>Amy.</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h2>Handleiding inbegrepen</h2>
      <p>Rafaël, Joris, Amy en Nicky.
      </p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h2>Simpel en veilig te gebruiken</h2>
      <p>Amy.</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h2>Worden er één of meerdere leerlijnen geraakt</h2>
      <p>Marc en Nicky.</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h2>Niet alleen willen klimmen ook ander opties</h2>
      <p>Amy.</p>
    </div>
  </div>
  <div class="container right">
    <div class="content">
      <h2>Verschillende wanden</h2>
      <p>Luca, Mariec, Joris en Marc.</p>
    </div>
  </div>
  <div class="container left">
    <div class="content">
      <h2>Beloning</h2>
      <p>Luca en Rafaël.</p>
    </div>
  </div>
  <div class="spacer"></div>
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
    margin-bottom: -50px;
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
