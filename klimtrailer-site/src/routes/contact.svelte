<script>
  let currentDate = new Date();

  let students = [
    {
      name: "Britney Janssen",
      email: "britney.janssen@student.fontys.nl",
      role: "Notulist",
    },
    {
      name: "Loes Käller",
      email: "l.kaller@student.fontys.nl",
      role: "Contactpersoon",
    },
    {
      name: "Matthijs de Vries",
      email: "m.devries@student.fontys.nl",
      role: "Teamlid",
    },
    {
      name: "Rick Peters",
      email: "r.peters-ab@student.fontys.nl",
      role: "Teamleider",
    },
    {
      name: "Stan Jaworski",
      email: "s.jaworski@student.fontys.nl",
      role: "Scrum Master",
    },
    {
      name: "Wout Ploumen",
      email: "w.ploumen@student.fontys.nl",
      role: "Teamlid",
    },
  ];
</script>

<svelte:head>
  <title>Contact</title>
</svelte:head>

<img src="images/groepsfoto.jpg" alt="Groeps Foto" width="100%" />

<main>
  <div class="left-bar" />
  <div class="content">
    <div class="gegevens">
      <h1>Contact</h1>

      <div class="gegevens-container">
        <p>Studenten</p>
        <div class="gegevens-column">
          {#each students as student}
            <div class="gegevens-item">
              <p><b>Naam:</b> {student.name}</p>
              <p>
                <b>Email:</b>
                <a href="mailto:{student.email}">{student.email}</a>
              </p>
              <p><b>Rol:</b> {student.role}</p>
            </div>
          {/each}
        </div>
        <div class="gegevens-column">

        </div>
      </div>
    </div>
  </div>
  <div class="right-bar" />
</main>

<style>
  main {
    display: grid;
    grid-template-columns: 25% 50% 25%;
    grid-auto-flow: column;
  }

  .gegevens-column {
    display: grid;
    grid-template-columns: 55% 45%;
    margin-bottom: 16px;
  }

  .gegevens-container p {
    margin-top: 0px;
    color: #f06119;
    font-weight: bold;
    margin-bottom: 4px;
  }

  .gegevens-item {
    margin-bottom: 16px;
  }

  .gegevens-item p {
    color: black;
    font-weight: normal;
    margin-top: 0px;
    margin-bottom: 0px;
  }
</style>
