<script>
  let personas = [
    {
      name: "Luca Jansen",
      desc: "Vrienden kun je ook online maken!",
      photoSrc: "/images/personas/lucajansen.png",
      age: 9,
      title: "Basisschoolleerling",
      link: "https://www.canva.com/design/DAEtPv0itnY/zspfQ6XYdnOOv1jhPNU68Q/view?utm_content=DAEtPv0itnY&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton",
    },
    {
      name: "Mariec Driesen",
      desc: "Een dag niet gezongen is een dag niet geleefd.",
      photoSrc: "/images/personas/mariecdriesen.png",
      age: 10,
      title: "Basisschoolleerling",
      link: "https://www.canva.com/design/DAEr1t2lMHg/u91L-lxsqVcgxPcqzt4t2A/view?utm_content=DAEr1t2lMHg&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton",
    },
    {
      name: "Casper de Haan",
      desc: "Je moet schieten, anders kun je niet scoren.",
      photoSrc: "/images/personas/casperdehaan.png",
      age: 7,
      title: "Basisschoolleerling",
      link: "https://www.canva.com/design/DAEreuYOfSM/4NQeh_qXpAVuTW4fbRHK_Q/view?utm_content=DAEreuYOfSM&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton",
    },
    {
      name: "Rafaël Manik Mas",
      desc: "Je bent moediger dan je gelooft, sterker dan je eruit ziet en slimmer dan je denkt. -Winnie de Poeh",
      photoSrc: "/images/personas/rafaelmanikmas.png",
      age: 12,
      title: "Basisschoolleerling",
      link: "https://www.canva.com/design/DAEsiir5JMo/8fZxJXK6IadDJ8KcS6S7JA/view?utm_content=DAEsiir5JMo&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton",
    },
    {
      name: "Joris Reiners",
      desc: "Het mooiste aan docent zijn op een basisschool is dat ik mag werken met een bak aan jong talent.",
      descStyle: "font-size: 15px;",
      photoSrc: "/images/personas/jorisreiners.png",
      age: 31,
      title: "Gymdocent",
      link: "https://www.canva.com/design/DAEtPohAUOc/v4TR0wwhv61nGh99tpIfhA/view?utm_content=DAEtPohAUOc&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton",
    },
    {
      name: "Nicky de Vries",
      desc: "Geef nooit op! Zet door, ook als het moeilijk wordt.",
      photoSrc: "/images/personas/nickydevries.png",
      age: 27,
      title: "Gymdocente",
      link: "https://www.canva.com/design/DAEr2IJVsPg/uMN8OPW9GPWJySq6ujEiUg/view?utm_content=DAEr2IJVsPg&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton",
    },
    {
      name: "Marc de Groot",
      desc: "De kinderen moeten zichzelf ontwikkelen en uitzoeken wat zij het leukste vinden om te doen.",
      photoSrc: "/images/personas/marcdegroot.png",
      age: 37,
      title: "Buurtsportcoach",
      link: "https://www.canva.com/design/DAEvUDWt0UQ/k19eQrurDIZhiU3uW9FxPg/view?utm_content=DAEvUDWt0UQ&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton",
    },
    {
      name: "Amy Ankers",
      desc: "Ik vind het belangrijk dat ik de kinderen enthousiast kan maken met de nieuwe kennis die ze van mij kunnen leren.",
      descStyle: "font-size: 14px;",
      photoSrc: "/images/personas/amyankers.png",
      age: 26,
      title: "Docent Basisschool",
      link: "https://www.canva.com/design/DAEvUJI94Dg/rHhWQ7mzyNO2QYX8XhtwMA/view?utm_content=DAEvUJI94Dg&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton",
    },
  ];

  let showModal = true;
  let currentId = undefined;

  function onPersonaClick(id) {
    currentId = id;
    showModal = true;
    console.log(currentId);
  }

  function hideModal() {
    showModal = false;
  }
</script>

<svelte:head>
  <title>Persona's</title>
</svelte:head>

<div class="main">
  <div class="content-pers">
    {#each personas as persona, id}
      <div
        class="item item-1"
        on:click={() => {
          onPersonaClick(id);
        }}
      >
        <img class="item-img" src={persona.photoSrc} alt={persona.name} />
        <div class="item-text">
          <p class="item-name">{persona.name}</p>
          <p class="item-dsc" style={persona.descStyle}>"{persona.desc}"</p>
        </div>
        <button class="item-btn">Meer informatie</button>
      </div>
    {/each}
  </div>
</div>
{#if showModal && currentId != undefined}
  <div class="persona-backdrop" on:click={hideModal} />

  <div class="persona-modal">
    <div class="upperbar">
      <i class="fa-solid fa-xmark" on:click={hideModal} />
    </div>
    <div class="modal-content">
      <h1 class="persona-name">{personas[currentId].name}</h1>
      <a href={personas[currentId].link} target="_blank">Link naar Canva</a>
      <h4 class="persona-title">
        {personas[currentId].title} ({personas[currentId].age} jaar oud)
      </h4>
      {#if currentId == 0}
        <p style="color: #F06119; display: inline;">Beschrijving</p>
        <p>
          Luca is graag samen met zijn klasgenootjes bezig, houdt van onderling
          contact en hij zou er graag een wedstrijdelement in terugzien. Zo zou
          hij ook graag willen dat het op een langer termijn leuk blijft. Luca
          heeft namelijk geen goed doorzettingsvermogen en vindt hierdoor dingen
          minder lang leuk.
        </p>

        <p style="color: #F06119; display: inline;">
          Hoe reageert hij op ons product?
        </p>
        <p>
          Luca ziet het nieuwe klimtoestel staan. Dingen als “dit ziet er best
          spannend uit” en “Dit kan ik niet” komen in Luca’s gedachten voorbij.
          Desondanks is hij ook wel een beetje nieuwsgierig erna. Wanneer het
          Luca’s beurt is om te klimmen geeft hij bij de juffrouw/meester aan
          dat hij het niet kan. Zodra hij wil opgeven legt de juffrouw/meester
          uit dat hij ook een iets simpelere route kan klimmen. De
          juffrouw/meester laat Luca merken dat zij/hij ervan overtuigd is dat
          Luca het kan. Luca is bezig met klimmen en komt erachter dat hij het
          stiekem ontzettend leuk vindt! Hij kan daarom ook niet wachten tot hij
          weer aan de beurt is. Zodra Luca tot het einde aangekomen is gaan er
          diverse lampjes branden, op deze manier wordt hij beloond voor zijn
          goede inzet. Gelukkig kan de klimwand op diverse manieren ingesteld
          worden waardoor het een uitdaging blijft voor Luca om zichzelf telkens
          te verbeteren en het niet saai wordt.
        </p>
        <p>
          Als de klimwand buiten in de volle zon gebruikt wordt kan Luca niet te
          lang meedoen doordat hij last heeft van een lichte zonneallergie. De
          juffrouw/meester moet hier rekening mee houden door hem onder een
          overkapping te zetten.
        </p>
      {:else if currentId == 1}
        <p style="color: #F06119; display: inline;">Beschrijving</p>
        <p>
          Voor Mariec maakt het niet zoveel uit of er wel of niet meerdere
          kinderen samen het product kunnen gebruiken. Zij heeft toch maar één
          zelfde schoolvriendin elke dag.
        </p>

        <p style="color: #F06119; display: inline;">
          Hoe reageert zij op ons product?
        </p>
        <p>
          Mariec kijkt samen met haar beste vriendin naar het schoolplein.
          Opeens ziet ze de nieuwe boulderwand. Samen kijken ze er naar uit om
          te gaan boulderen in de gymles. Gelukkig is het apparaat
          multifunctioneel. Er kan ook een bankje worden in gehangen. Voor
          Mariec is het belangrijk dat er niet teveel kinderen tegelijk op de
          boulderwand klimmen, als er teveel andere klasgenoten tegelijk klimmen
          wordt ze verlegen en vindt ze het niet meer leuk. Tijdens de gymles
          komt Mariec er al snel achter dat het te makkelijk is voor haar.
          Gelukkig kan het apparaat verschillende moeilijkheid niveaus aan en
          kan de kantel hoek worden veranderd. Dit zorgt voor een grotere
          motivatie en doorzetting vermogen. De hoogte van het apparaat zorgt
          ervoor dat het een adrenaline kick geeft. Na de gymles kijkt Mariec en
          haar best vriendin er weer naar uit de volgende les het te gaan
          gebruiken. Gelukkig zijn ze deze gymles wel vermoeid. Dit voelde als
          een uitdagende gymles.
        </p>
      {:else if currentId == 2}
        <p style="color: #F06119; display: inline;">Beschrijving</p>
        <p>
          Casper is erg fanatiek en nieuwsgierig. Van een nieuw gymtoestel wordt
          hij dan ook erg enthousiast. Het kan voor Casper allemaal niet gek
          genoeg zijn.
        </p>

        <p style="color: #F06119; display: inline;">
          Hoe reageert hij op ons product?
        </p>
        <p>
          Casper heeft vorige week de klimwand in de berging zien staan en heeft
          toen aan de juffrouw/meester gevraagd wanneer ze die tijdens de gymles
          zouden gebruiken. Hij wil hier heel graag op klimmen. Hij loopt
          vandaag de gymles in en hij ziet de klimwand staan en hij kan zijn
          geluk niet op. Hij vraagt gelijk aan de docent hoe hoog ze gaan
          klimmen, want als het aan Casper ligt klimt hij gelijk helemaal naar
          de top. Dan kan hij dit vanavond vol trots tijdens de training
          vertellen aan zijn teamgenootjes. Helaas zegt de juffrouw/meester dat
          ze vandaag rustig aan zullen beginnen en misschien over een paar weken
          hoger zullen gaan, Casper baalt hiervan maar staat des al niet te min
          vooraan als de juffrouw/meester zegt dat ze gaan beginnen. Casper
          klimt met speels gemak omhoog en laat even goed zien aan de rest hoe
          het moet. Casper komt beneden en vindt het super leuk, hij kan niet
          wachten tot ze dit volgende week weer gaan doen. Maar dan wilt hij het
          liefste wel een stukje hoger.
        </p>
      {:else if currentId == 3}
        <p style="color: #F06119; display: inline;">Beschrijving</p>
        <p>
          Rafaël kijkt bij een nieuw toestel liever eerst even de kat uit de
          boom. Daarnaast ontvangt hij graag ondersteuning van de docent als het
          even moeilijk wordt. Rafaël moet tevens telkens opnieuw worden
          uitgedaagd om het leuk te blijven vinden.
        </p>

        <p style="color: #F06119; display: inline;">
          Hoe reageert hij op ons product?
        </p>
        <p>
          Rafaël komt de gymles binnen en ziet iets wat hij nog niet eerder
          gezien heeft. Het lijkt op een klimmuur maar hij weet nog niet zo goed
          wat ze ermee gaan doen tijdens de les, hij hoort het zo wel van de
          juffrouw/meester. De juffrouw/meester vertelt de klas dat ze in een
          rij moeten gaan staan, Rafaël gaat samen met zijn beste vrienden in
          het midden staan, hij wil eerst even rustig kijken hoe dit moet
          voordat hij zelf gaat klimmen. Hij ziet dat de ene het moeilijker
          vindt dan de ander. Wel merkt hij dat de juffrouw/meester aanwijzingen
          geeft als iemand even niet zo goed weet wat hij/zij moet doen, dat
          vindt Rafaël fijn. Dan is hij aan de beurt, hij vindt het spannend
          maar hij denkt wel dat hij dit kan, hij is namelijk iets langer dan
          zijn klasgenoten en kan er dus makkelijker bij. De eerste paar punten
          gaan lastig maar dan begint hij er steeds meer gevoel voor te krijgen.
          Alleen bij de laatste loopt hij vast, gelukkig geeft de
          juffrouw/meester een tip waardoor hij het einde haalt en hij daarna
          weer veilig naar beneden klimt. Hij heeft het gedaan en het ging goed,
          als beloning krijgt hij high-fives van zijn vrienden. Echter denkt
          Rafaël dat hij het de volgende keer wel zonder de hulp van de
          juffrouw/meester kan. Hij kan het nu, het is hem namelijk gelukt. De
          volgende keer zal de klimmuur dus gaan vervelen en zal hij opnieuw
          uitgedaagd moeten worden.
        </p>
      {:else if currentId == 4}
        <p style="color: #F06119; display: inline;">Beschrijving</p>
        <p>
          Joris vindt het belangrijk dat het product veilig genoeg is voor de
          kinderen. Hij wil ook kinderen persoonlijk aandacht kunnen geven.
          Sommige kinderen durven niet te klimmen en lopen erg achter met hun
          motoriek. Er zou een product moeten zijn dat multifunctioneel is.
        </p>

        <p style="color: #F06119; display: inline;">
          Hoe reageert hij op ons product?
        </p>
        <p>
          Hij kan goed omgaan met kinderen zoals Luca, maar ook met kinderen
          zoals Rafaël. Hij weet beiden goed te motiveren en aan te sporen.
          Joris heeft zijn zaken altijd op orde en is voorbereid. Als het op de
          klimwand aankomt weet hij dus goed wat er op hem staat te wachten, hij
          heeft het namelijk al tot in de puntjes uitgezocht. Joris doet graag
          dingen die hij zelf ook leuk vindt om te doen. Wanneer Joris een
          minder leuk toestel tegenkomt, bedenkt hij samen met de kinderen of de
          kinderen bedenken er alleen een leuke spelvorm bij. Hierdoor sluiten
          de lessen beter aan bij de belevingen en niveaus van zijn eigen
          leerlingen. Joris is erg geduldig en weet de juiste manier toe te
          passen om het voor iedereen leuk te maken.
        </p>
      {:else if currentId == 5}
        <p style="color: #F06119; display: inline;">Beschrijving</p>
        <p>
          Nicky verdiept zich altijd erg goed in de mogelijkheden van haar
          gymles. Ze weet tevens welk niveau ieder individueel kind aankan. Het
          product moet daarom verstelbaar zijn per niveau dat bij het kind
          aansluit om de leerdoelen te kunnen behalen.
        </p>

        <p style="color: #F06119; display: inline;">
          Hoe reageert hij op ons product?
        </p>
        <p>
          Dankzij de goede expertise en onderzoeken die Nicky doet weet ze
          direct wat ze met de klimwand moet doen. Van iedere leerling weet
          Nicky op welk niveau ze kunnen klimmen. Ze vindt het tevens erg leuk
          om iets nieuws uit te proberen tijdens haar lessen. Daarnaast vindt ze
          het ook fijn dat ze zelf de indelingen kan bepalen van de klimwand,
          dit houdt ook haar goed bezig. Ze kan er goed voor zorgen dat de
          kinderen plezier hebben tijdens het klimmen en dat ze de juiste
          leerdoelen weten te behalen. Nicky wordt erg vrolijk en enthousiast
          van kinderen zoals Casper.
        </p>
        <p>
          Naast schooltijd geeft ze ook tennisles, dit laat zien dat ze het
          belangrijk vindt dat de kinderen ook na schooltijd actief bezig zijn.
        </p>
      {:else if currentId == 6}
        <p style="color: #F06119; display: inline;">Beschrijving</p>
        <p>
          Marc vindt de verbinding tussen de kinderen waarschijnlijk het aller
          belangrijkste. Meerdere kinderen moeten om deze reden tegelijkertijd
          met het product aan de slag kunnen.
        </p>

        <p style="color: #F06119; display: inline;">
          Hoe reageert hij op ons product?
        </p>
        <p>
          Marc is vanuit de gemeente aangenomen als buurtsportcoach en is via
          detachering werkzaam op diverse basisscholen om gymles te geven.
        </p>
        <p>
          Marc vindt het belangrijk dat de kinderen goed hun energie kwijt
          kunnen tijdens de gymlessen. Hij vindt het dan ook belangrijk dat er
          genoeg variatie zit in de les, zodat de kinderen zichzelf goed kunnen
          ontwikkelen. Met de klimwand is dit uiteraard goed mogelijk en vindt
          hij daarom ook erg fijn in gebruik. De klimwand is namelijk
          multifunctioneel en kan op veel verschillende manieren ingezet worden.
          Kinderen zoals Luca kan hij soms overvallen met informatie, omdat hij
          het jammer vindt als men vooraf al zegt dat men iets niet kan.
          Desondanks maakt hij kinderen als Casper alleen maar fanatieker door
          zijn toespraken.
        </p>
        <p>
          Marc vindt het tevens belangrijk dat de kinderen deelnemen aan de
          vereniging die hij na schooltijd organiseert.
        </p>
      {:else if currentId == 7}
        <p style="color: #F06119; display: inline;">Beschrijving</p>
        <p>
          Amy wil graag zo makkelijk mogelijk gymles kunnen geven. De materialen
          moeten niet moeilijk op te zetten zijn en de kinderen moeten zichzelf
          goed bezig kunnen houden. Daarnaast valt Amy snel terug op
          activiteiten waar ze reeds mee bekend is.
        </p>

        <p style="color: #F06119; display: inline;">
          Hoe reageert hij op ons product?
        </p>
        <p>
          Voor Amy moeten de gymlessen zo makkelijk en veilig mogelijk zijn,
          aangezien ze geen tijd en moeite wil steken in het opzetten van
          allerlei materialen en ongelukken wil voorkomen. De klimwand moet dan
          ook makkelijk binnen handbereik zijn. Dankzij de makkelijke App kan ze
          goed een nieuwe route aanvinken voor een andere leerling zonder er al
          te veel moeite in te hoeven steken. Ze vindt het niet erg als een kind
          niet wil klimmen, want dan is ze zelf ongerust dat het kind wellicht
          gaat vallen. Gelukkig is de wand multifunctioneel en kunnen de
          kinderen die niet willen klimmen iets anders met de oorspronkelijke
          klimwand doen. Op deze manier kan ook Amy de muur goed gebruiken,
          doordat er niet te veel kinderen bij komen kijken hoe zij het doet.
          Juf Amy heeft gemerkt dat de kinderen vrijwel alles leuk vinden om te
          doen tijdens de gymles.
        </p>
      {/if}
    </div>
  </div>
{/if}

<style>
  .persona-backdrop {
    position: fixed;
    top: 0;
    left: 0;
    height: 100%;
    background-color: rgba(33, 37, 41, 0.3);
    width: 100%;
    z-index: 998;
  }

  .upperbar {
    height: 32px;
    border-bottom: 1px solid #4a4a55;
  }

  .persona-modal {
    position: fixed;
    background-color: white;
    box-shadow: 0 2px 4px 0 rgba(0, 0, 0, 0.2);
    border: 1px solid #4a4a55;
    border-radius: 4px;
    top: 50%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    z-index: 999;
    max-width: 35%;
    max-height: 90%;
    overflow-y: auto;
  }

  @media (max-width: 1400px) {
    .persona-modal {
      max-width: 50%;
    }
  }

  @media (max-width: 1200px) {
    .persona-modal {
      max-width: 60%;
    }
  }

  @media (max-width: 1000px) {
    .persona-modal {
      max-width: 70%;
    }
  }

  .modal-content {
    padding: 8px 24px;
  }

  .modal-content p {
    text-align: justify;
    margin-top: 0px;
  }

  .fa-xmark {
    color: #4a4a55;
    font-size: 32px;
    float: right;
    margin-right: 5px;
  }

  .fa-xmark:hover {
    cursor: pointer;
    color: black;
  }

  .main {
    display: block;
  }

  .content-pers {
      display: grid;
      grid-template-rows: 405px 405px;
      grid-template-columns: 230px 230px 230px 230px;
      grid-gap: 15px;
      justify-content: center;
  }

  @media(min-width: 1669px){
    .content-pers {
      grid-template-rows: 405px 405px;
      grid-template-columns: 230px 230px 230px 230px;
    }
  }

  @media(max-width: 1668px){
    .content-pers {
      grid-template-rows: 405px 405px 405px;
      grid-template-columns: 230px 230px 230px;
    }
  }

  @media(max-width: 1500px){
    .content-pers {
      grid-template-rows: 405px 405px 405px 405px;
      grid-template-columns: 230px 230px;
    }
  }

  @media(max-width: 1349px){
    .content-pers {
      grid-template-rows: 405px 405px;
      grid-template-columns: 230px 230px 230px 230px;
    }
  }

  @media(max-width: 1000px){
    .content-pers {
      grid-template-rows: 405px 405px 405px 405px;
      grid-template-columns: 230px 230px;
    }
  }

  .item {
    margin: 8px;
    text-align: left;
    background-color: #ccd7ff;
    border-radius: 8px;
    cursor: pointer;
    z-index: 997;
  }

  .item:hover {
    border: 1px solid white;
  }

  .item-img {
    width: 100%;
    height: 214px;
    object-fit: fill;
    border-top-left-radius: 8px;
    border-top-right-radius: 8px;
  }

  .item-name {
    margin-top: 0px;
    margin-bottom: 0px;
    font-weight: bold;
    margin-left: 6px;
    font-size: 20px;
  }

  .item-dsc {
    margin-top: 2px;
    margin-left: 6px;
  }

  .item-text {
    padding-left: 4px;
    padding-right: 4px;
    padding-top: 4px;
    margin-top: -4px;
    height: 124px;
  }

  .item-btn {
    width: 100%;
    background-color: #004b8e;
    color: rgb(225, 225, 225);
    height: 32px;
    font-size: 16px;
    border: none;
    outline: none;
    border-bottom-left-radius: 8px;
    border-bottom-right-radius: 8px;
    cursor: pointer;
    margin-top: 15px;
  }

  .persona-name {
    margin-top: 0px;
    margin-bottom: 0px;
    margin-right: 16px;
    display: inline;
  }

  .persona-title {
    margin-top: 0px;
  }
</style>
