<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Merkspiel</title>

<style>

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  min-height: 100vh;
  font-family: Arial, sans-serif;
  background: #f2f0e8;
  color: #222;
}

.app {
  max-width: 430px;
  margin: auto;
  padding: 16px 14px;
}


/* =========================================
   EINSTELLUNGEN
========================================= */

.settings {
  background: #fff;
  padding: 15px;
  border-radius: 14px;
  box-shadow: 0 2px 9px #0002;
}

label {
  display: block;
  font-weight: bold;
  margin: 10px 0 5px;
}

select,
button {
  width: 100%;
  font-size: 18px;
  padding: 11px;
  border-radius: 10px;
}

select {
  border: 1px solid #aaa;
  background: #fff;
}

button {
  margin-top: 14px;
  border: 0;
  background: #222;
  color: #fff;
  font-weight: bold;
  cursor: pointer;
  -webkit-tap-highlight-color: transparent;
}

button:active {
  transform: scale(0.98);
}


/* =========================================
   SPIEL
========================================= */

.game {
  display: none;
  text-align: center;
}

.phase {
  font-size: 21px;
  font-weight: bold;
  margin-top: 15px;
}

.timer {
  font-size: 48px;
  font-weight: bold;
  margin: 3px;
}

.hint {
  font-size: 15px;
  margin: 4px 0 12px;
}


/* =========================================
   SPIELFELD
========================================= */

.grid {
  width: min(92vw, 330px);
  margin: auto;

  display: grid;

  grid-template-columns:
    repeat(4, 1fr);

  gap: 8px;
}

.tile {
  aspect-ratio: 1;

  background: #b8b8b8;

  border-radius: 12px;

  display: flex;

  align-items: center;
  justify-content: center;

  font-weight: bold;

  font-size:
    clamp(26px, 8vw, 38px);

  box-shadow:
    0 2px 6px #0003;

  overflow: hidden;

  position: relative;

  user-select: none;
}


/* =========================================
   ZAHLEN
========================================= */

.number {
  color: #0645ad;
  font-weight: 900;
}


/* =========================================
   SYMBOLE
========================================= */

.symbol {
  color: #a00000;
  font-weight: 900;
}


/* =========================================
   FARBEN
========================================= */

.color-circle {
  width: 62%;
  height: 62%;

  border-radius: 50%;

  border: 3px solid #222;

  display: block;
}

.circle-black {
  background: #000000;
}

.circle-white {
  background: #ffffff;
}

.circle-red {
  background: #e00000;
}

.circle-yellow {
  background: #ffd400;
}

.circle-green {
  background: #00a83b;
}

.circle-blue {
  background: #0066d6;
}

.circle-orange {
  background: #ff7a00;
}

.circle-purple {
  background: #7b22c9;
}

.circle-brown {
  background: #8b4a24;
}

.circle-pink {
  background: #f05a9d;
}


/* =========================================
   AUSGEWÄHLTES BILD
========================================= */

.tile.selected {

  background: #d7d7d7;

  box-shadow:
    0 0 0 4px #222 inset,
    0 2px 6px #0003;
}

.tile.selected::after {

  content: attr(data-number);

  position: absolute;

  right: 5px;
  top: 5px;

  min-width: 25px;
  height: 25px;

  border-radius: 50%;

  background: #222;

  color: white;

  font-size: 15px;

  display: flex;

  align-items: center;
  justify-content: center;
}


/* =========================================
   RICHTIG / FALSCH
========================================= */

.feedback {

  display: none;

  font-size: 38px;

  font-weight: 900;

  margin: 20px 0;

  min-height: 48px;
}

.feedback.wrong {
  color: #c00000;
}

.feedback.correct {
  color: #16832c;
}


/* =========================================
   ERGEBNIS
========================================= */

.result {

  display: none;

  margin-top: 18px;

  padding: 16px;

  border-radius: 14px;

  background: #fff;

  box-shadow:
    0 2px 9px #0002;
}

.result-message {

  font-size: 30px;

  font-weight: 900;

  margin-bottom: 12px;
}

.result.correct .result-message {
  color: #16832c;
}

.result.wrong .result-message {
  color: #c00000;
}

.result-info {

  font-size: 14px;

  color: #555;

  margin-bottom: 15px;
}

.comparison-title {

  font-size: 18px;

  font-weight: bold;

  margin-bottom: 8px;
}

.comparison-label {

  font-size: 13px;

  font-weight: bold;

  margin-top: 12px;

  margin-bottom: 5px;
}

.small-grid {

  width: 100%;

  display: grid;

  grid-template-columns:
    repeat(4, 1fr);

  gap: 5px;
}

.small-grid .tile {

  font-size: 22px;

  border-radius: 7px;
}

.small-grid .color-circle {

  width: 60%;
  height: 60%;

  border-width: 2px;
}

.small-grid .tile.selected::after {

  font-size: 10px;

  min-width: 17px;
  height: 17px;

  right: 2px;
  top: 2px;
}


/* =========================================
   ZURÜCK
========================================= */

.secondary {

  background: #fff;

  color: #222;

  border: 1px solid #888;

  margin-top: 15px;
}

</style>
</head>


<body>

<div class="app">


<!-- =====================================
     EINSTELLUNGEN
===================================== -->

<div
  class="settings"
  id="settings">


<label for="type">
  Thema
</label>

<select id="type">

  <option value="numbers">
    Zahlen
  </option>

  <option value="colors">
    Farben
  </option>

  <option value="symbols">
    Symbole
  </option>

  <option value="mixed">
    Gemischt
  </option>

</select>


<label for="memory">
  Zeit zum Merken
</label>

<select id="memory">

  <option value="10">
    10 Sekunden
  </option>

  <option value="15">
    15 Sekunden
  </option>

  <option value="20">
    20 Sekunden
  </option>

  <option value="25">
    25 Sekunden
  </option>

  <option value="30">
    30 Sekunden
  </option>

</select>


<label for="count">
  Anzahl der Bilder
</label>

<select id="count">

  <option value="4">4</option>
  <option value="5">5</option>
  <option value="6">6</option>
  <option value="7">7</option>
  <option value="8">8</option>
  <option value="9">9</option>
  <option value="10">10</option>

</select>


<label for="duplicates">
  Bilder
</label>

<select id="duplicates">

  <option value="unique">
    Nur einzeln
  </option>

  <option value="duplicates">
    Doppelte möglich
  </option>

</select>


<label for="solve">
  Zeit
</label>

<select id="solve">

  <option value="30">
    30 Sekunden
  </option>

  <option value="45">
    45 Sekunden
  </option>

  <option value="60">
    60 Sekunden
  </option>

  <option value="75">
    75 Sekunden
  </option>

  <option value="90">
    90 Sekunden
  </option>

</select>


<button
  type="button"
  id="startButton">

  Neue Runde starten

</button>


</div>


<!-- =====================================
     SPIEL
===================================== -->

<div
  class="game"
  id="game">


<div
  class="phase"
  id="phase">
</div>


<div
  class="timer"
  id="timer">
</div>


<div
  class="hint"
  id="hint">
</div>


<div
  class="feedback"
  id="feedback">
</div>


<div
  class="grid"
  id="grid">
</div>


<!-- =====================================
     ERGEBNIS
===================================== -->

<div
  class="result"
  id="result">


<div
  class="result-message"
  id="resultMessage">
</div>


<div
  class="result-info"
  id="resultInfo">
</div>


<div class="comparison-title">
  Vergleich
</div>


<div class="comparison-label">
  Richtige Lösung
</div>


<div
  class="small-grid"
  id="solutionGrid">
</div>


<div class="comparison-label">
  Deine Eingabe
</div>


<div
  class="small-grid"
  id="answerGrid">
</div>


<button
  type="button"
  class="secondary"
  id="backButton">

  Neue Runde

</button>


</div>


</div>


</div>


<script>


/* =========================================
   VARIABLEN
========================================= */

let sequence = [];

let selectionPool = [];

let playerAnswer = [];

let attempts = 0;

let interval = null;

let acceptingInput = false;


/* =========================================
   ELEMENTE
========================================= */

const settings =
  document.getElementById("settings");

const game =
  document.getElementById("game");

const typeSelect =
  document.getElementById("type");

const memorySelect =
  document.getElementById("memory");

const countSelect =
  document.getElementById("count");

const duplicatesSelect =
  document.getElementById("duplicates");

const solveSelect =
  document.getElementById("solve");

const startButton =
  document.getElementById("startButton");

const backButton =
  document.getElementById("backButton");

const phase =
  document.getElementById("phase");

const timer =
  document.getElementById("timer");

const hint =
  document.getElementById("hint");

const grid =
  document.getElementById("grid");

const feedback =
  document.getElementById("feedback");

const result =
  document.getElementById("result");

const resultMessage =
  document.getElementById("resultMessage");

const resultInfo =
  document.getElementById("resultInfo");

const solutionGrid =
  document.getElementById("solutionGrid");

const answerGrid =
  document.getElementById("answerGrid");


/* =========================================
   ZAHLEN
========================================= */

const numbers = [

  "0",
  "1",
  "2",
  "3",
  "4",
  "5",
  "6",
  "7",
  "8",
  "9"

];


/* =========================================
   SYMBOLE
========================================= */

const symbols = [

  "★",
  "■",
  "●",
  "=",
  "♥",
  "◆",
  "➜",
  "+",
  "−",
  "×"

];


/* =========================================
   FARBEN
========================================= */

const colors = [

  {
    name: "Schwarz",
    className: "circle-black"
  },

  {
    name: "Weiß",
    className: "circle-white"
  },

  {
    name: "Rot",
    className: "circle-red"
  },

  {
    name: "Gelb",
    className: "circle-yellow"
  },

  {
    name: "Grün",
    className: "circle-green"
  },

  {
    name: "Blau",
    className: "circle-blue"
  },

  {
    name: "Orange",
    className: "circle-orange"
  },

  {
    name: "Lila",
    className: "circle-purple"
  },

  {
    name: "Braun",
    className: "circle-brown"
  },

  {
    name: "Rosa",
    className: "circle-pink"
  }

];


/* =========================================
   POOL
========================================= */

function pool(type) {

  if (type === "numbers") {

    return numbers.map(function(x) {

      return {
        v: x,
        kind: "number"
      };

    });

  }


  if (type === "symbols") {

    return symbols.map(function(x) {

      return {
        v: x,
        kind: "symbol"
      };

    });

  }


  if (type === "colors") {

    return colors.map(function(x) {

      return {
        v: x.className,
        label: x.name,
        kind: "color"
      };

    });

  }


  return [

    ...numbers.map(function(x) {

      return {
        v: x,
        kind: "number"
      };

    }),

    ...symbols.map(function(x) {

      return {
        v: x,
        kind: "symbol"
      };

    }),

    ...colors.map(function(x) {

      return {
        v: x.className,
        label: x.name,
        kind: "color"
      };

    })

  ];

}


/* =========================================
   MISCHEN
========================================= */

function shuffle(array) {

  const a = [...array];

  for (
    let i = a.length - 1;
    i > 0;
    i--
  ) {

    const j =
      Math.floor(
        Math.random() * (i + 1)
      );

    const temp =
      a[i];

    a[i] =
      a[j];

    a[j] =
      temp;

  }

  return a;

}


/* =========================================
   SEQUENZ
========================================= */

function makeSequence(type, n) {

  const p =
    pool(type);

  if (
    duplicatesSelect.value ===
    "unique"
  ) {

    return shuffle(p)
      .slice(0, n);

  }

  const a = [];

  for (
    let i = 0;
    i < n;
    i++
  ) {

    const index =
      Math.floor(
        Math.random() *
        p.length
      );

    a.push(
      p[index]
    );

  }

  return a;

}


/* =========================================
   VERGLEICH
========================================= */

function sameItem(a, b) {

  if (!a || !b) {
    return false;
  }

  return (
    a.v === b.v &&
    a.kind === b.kind
  );

}


/* =========================================
   BILD ERSTELLEN
========================================= */

function createTile(x) {

  const d =
    document.createElement("div");

  d.className =
    "tile";


  if (
    x.kind === "number"
  ) {

    d.classList.add(
      "number"
    );

    d.textContent =
      x.v;

  }


  else if (
    x.kind === "symbol"
  ) {

    d.classList.add(
      "symbol"
    );

    d.textContent =
      x.v;

  }


  else if (
    x.kind === "color"
  ) {

    const circle =
      document.createElement(
        "div"
      );

    circle.className =
      "color-circle " +
      x.v;

    d.appendChild(
      circle
    );

    d.title =
      x.label;

  }


  return d;

}


/* =========================================
   FELD ZEICHNEN
========================================= */

function draw(el, array) {

  el.innerHTML =
    "";

  array.forEach(
    function(x) {

      el.appendChild(
        createTile(x)
      );

    }
  );

}


/* =========================================
   IMMER 10 AUSWAHLBILDER
========================================= */

function makeSelectionPool() {

  const p =
    pool(
      typeSelect.value
    );

  let choices =
    [...sequence];


  const available =
    p.filter(
      function(item) {

        return !sequence.some(
          function(correct) {

            return sameItem(
              item,
              correct
            );

          }
        );

      }
    );


  const wrong =
    shuffle(
      available
    );


  while (
    choices.length < 10 &&
    wrong.length > 0
  ) {

    choices.push(
      wrong.shift()
    );

  }


  while (
    choices.length < 10
  ) {

    const randomItem =
      p[
        Math.floor(
          Math.random() *
          p.length
        )
      ];

    choices.push(
      randomItem
    );

  }


  return shuffle(
    choices.slice(0, 10)
  );

}


/* =========================================
   AUSWAHLFELD
========================================= */

function drawSelectionGrid() {

  grid.innerHTML =
    "";

  selectionPool.forEach(
    function(item, index) {

      const tile =
        createTile(item);

      tile.dataset.index =
        index;

      tile.addEventListener(
        "click",
        function() {

          selectTile(
            tile,
            index
          );

        }
      );

      grid.appendChild(
        tile
      );

    }
  );

}


/* =========================================
   BILD AUSWÄHLEN
========================================= */

function selectTile(tile, index) {

  if (!acceptingInput) {
    return;
  }

  if (
    tile.classList.contains(
      "selected"
    )
  ) {

    return;

  }

  const number =
    playerAnswer.length + 1;


  tile.classList.add(
    "selected"
  );

  tile.dataset.number =
    number;


  playerAnswer.push(
    selectionPool[index]
  );


  /*
     SOFORT PRÜFEN:
     Ist das gerade gewählte Bild
     an dieser Stelle falsch?
  */

  const position =
    playerAnswer.length - 1;


  if (
    !sameItem(
      playerAnswer[position],
      sequence[position]
    )
  ) {

    wrongAnswer();

    return;

  }


  /*
     Alle Bilder richtig
  */

  if (
    playerAnswer.length ===
    sequence.length
  ) {

    correctAnswer();

  }

}


/* =========================================
   FALSCH
========================================= */

function wrongAnswer() {

  acceptingInput =
    false;

  clearInterval(
    interval
  );

  interval =
    null;


  feedback.textContent =
    "Falsch";

  feedback.className =
    "feedback wrong";

  feedback.style.display =
    "block";


  /*
     FALSCH bleibt genau
     zwei Sekunden sichtbar.
  */

  setTimeout(
    function() {

      feedback.style.display =
        "none";


      attempts++;


      /*
         Nach dem ersten falschen
         Versuch gibt es genau noch
         EINEN Versuch.
      */

      if (
        attempts === 1
      ) {

        startLastAttempt();

      }

      else {

        showResult(
          false
        );

      }

    },
    2000
  );

}


/* =========================================
   RICHTIG
========================================= */

function correctAnswer() {

  acceptingInput =
    false;

  clearInterval(
    interval
  );

  interval =
    null;

  attempts++;

  feedback.textContent =
    "Richtig!";

  feedback.className =
    "feedback correct";

  feedback.style.display =
    "block";


  setTimeout(
    function() {

      feedback.style.display =
        "none";

      showResult(
        true
      );

    },
    1000
  );

}


/* =========================================
   COUNTDOWN
========================================= */

function countdown(
  seconds,
  text,
  finished
) {

  clearInterval(
    interval
  );

  let t =
    seconds;


  phase.textContent =
    text;

  timer.textContent =
    t;


  interval =
    setInterval(
      function() {

        t--;

        timer.textContent =
          t;


        if (
          t <= 0
        ) {

          clearInterval(
            interval
          );

          interval =
            null;

          finished();

        }

      },
      1000
    );

}


/* =========================================
   START
========================================= */

function startGame() {

  clearInterval(
    interval
  );

  interval =
    null;

  attempts =
    0;

  playerAnswer =
    [];

  acceptingInput =
    false;


  const anzahl =
    Number(
      countSelect.value
    );


  sequence =
    makeSequence(
      typeSelect.value,
      anzahl
    );


  settings.style.display =
    "none";

  game.style.display =
    "block";

  result.style.display =
    "none";

  feedback.style.display =
    "none";


  hint.textContent =
    "Merke dir die Bilder in dieser Reihenfolge.";


  draw(
    grid,
    sequence
  );


  countdown(

    Number(
      memorySelect.value
    ),

    "Merken!",

    function() {

      showTwoAttemptsMessage();

    }

  );

}


/* =========================================
   NACH DER MERKZEIT
========================================= */

function showTwoAttemptsMessage() {

  clearInterval(
    interval
  );

  interval =
    null;


  phase.textContent =
    "Nur zwei Versuche!";

  timer.textContent =
    "";

  hint.textContent =
    "";

  grid.innerHTML =
    "";


  /*
     Der Hinweis wird zwei Sekunden
     angezeigt.
  */

  setTimeout(
    function() {

      startFirstAttempt();

    },
    2000
  );

}


/* =========================================
   ERSTER VERSUCH
========================================= */

function startFirstAttempt() {

  playerAnswer =
    [];

  acceptingInput =
    true;


  selectionPool =
    makeSelectionPool();


  phase.textContent =
    "1. Versuch";


  hint.textContent =
    "Wähle die Bilder in der richtigen Reihenfolge.";


  drawSelectionGrid();


  countdown(

    Number(
      solveSelect.value
    ),

    "Zeit!",

    function() {

      if (
        acceptingInput
      ) {

        acceptingInput =
          false;

        attempts++;

        showResult(
          false
        );

      }

    }

  );

}


/* =========================================
   LETZTER VERSUCH
========================================= */

function startLastAttempt() {

  playerAnswer =
    [];

  acceptingInput =
    true;


  selectionPool =
    makeSelectionPool();


  phase.textContent =
    "Nur ein Versuch!";


  timer.textContent =
    "";


  hint.textContent =
    "Letzter Versuch – wähle deine Bilder in der richtigen Reihenfolge.";


  drawSelectionGrid();


  countdown(

    Number(
      solveSelect.value
    ),

    "Zeit!",

    function() {

      if (
        acceptingInput
      ) {

        acceptingInput =
          false;

        attempts++;

        showResult(
          false
        );

      }

    }

  );

}


/* =========================================
   ERGEBNIS
========================================= */

function showResult(correct) {

  acceptingInput =
    false;

  clearInterval(
    interval
  );

  interval =
    null;


  phase.textContent =
    "Ergebnis";


  timer.textContent =
    "";


  grid.innerHTML =
    "";


  feedback.style.display =
    "none";


  if (correct) {

    result.className =
      "result correct";


    resultMessage.textContent =
      "Richtig!";


    resultInfo.textContent =
      "Geschafft – du hast " +
      attempts +
      " von 2 Versuchen benötigt.";

  }

  else {

    result.className =
      "result wrong";


    resultMessage.textContent =
      "Falsch";


    resultInfo.textContent =
      "Beide Versuche waren falsch.";

  }


  draw(
    solutionGrid,
    sequence
  );


  draw(
    answerGrid,
    playerAnswer
  );


  result.style.display =
    "block";


  hint.textContent =
    "Hier siehst du die richtige Lösung und deine Eingabe zum Vergleich.";

}


/* =========================================
   NEUE RUNDE
========================================= */

function backToSettings() {

  clearInterval(
    interval
  );

  interval =
    null;


  acceptingInput =
    false;


  game.style.display =
    "none";


  settings.style.display =
    "block";


  grid.innerHTML =
    "";


  solutionGrid.innerHTML =
    "";


  answerGrid.innerHTML =
    "";


  result.style.display =
    "none";


  feedback.style.display =
    "none";


  phase.textContent =
    "";


  timer.textContent =
    "";


  hint.textContent =
    "";

}


/* =========================================
   BUTTONS
========================================= */

startButton.addEventListener(
  "click",
  function() {

    startGame();

  }
);


backButton.addEventListener(
  "click",
  function() {

    backToSettings();

  }
);

</script>

</body>
</html>
