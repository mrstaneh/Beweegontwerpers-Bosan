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

<main>
    <div class="left-bar" />
    <div class="content">
        <div class="gegevens">
            <h1>Gegevens</h1>

            <div class="gegevens-container">
                <div class="gegevens-column">
                <p>Studenten</p>
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
                <p>Verslag</p>
                <div class="gegevens-item">
                    <p><b>Titel:</b> ........</p>
                    <p><b>Versie:</b> 1</p>
                    <p>
                    <b>Datum:</b>
                    {currentDate.getDay()}-{currentDate.getMonth()}-{currentDate.getFullYear()}
                    </p>
                </div>

                <p style="margin-top: 54px;">Bedrijf</p>
                <div class="gegevens-item">
                    <p><b>Naam:</b> Bosan B.V.</p>
                    <p><b>Adres:</b> Metaalstraat 21, 7483 PD Haaksbergen</p>
                    <p><b>Telefoonnummer:</b> 053-3035107</p>
                </div>

                <p style="margin-top: 54px;">Opdrachtgever</p>
                <div class="gegevens-item">
                    <p><b>Contactpersoon:</b> Mark Snijder</p>
                    <p>
                    <b>E-mail:</b>
                    <a href="mailto:m.snijder@bosan.nl">m.snijder@bosan.nl</a>
                    </p>
                    <p><b>Mobiel telefoonnummer:</b> 06-21246905</p>
                </div>

                <p style="margin-top: 54px;">Opdrachtgever</p>
                <div class="gegevens-item">
                    <p><b>Contactpersoon:</b> Melanie van Deursen</p>
                    <p>
                    <b>E-mail:</b>
                    <a href="mailto:m.vandeursen@groupe-abeo.com"
                        >m.vandeursen@groupe-abeo.com</a
                    >
                    </p>
                </div>
                </div>
            </div>
            <img class="gegevens-image" src="bosan-2.jpg" alt="" />
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

    .gegevens-container {
        display: grid;
        grid-template-columns: 55% 45%;
        grid-auto-flow: column;
        margin-bottom: 16px;
    }

    .gegevens-column p {
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

    .gegevens-image {
        width: 100%;
    }
</style>