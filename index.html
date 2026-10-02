<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Total Verschnurrt – Raum 4</title>
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
  width: 100%;
  max-width: 500px;
  margin: auto;
  padding: 16px;
}
.header {
  text-align: center;
  margin-bottom: 16px;
}
.title {
  font-size: 30px;
  font-weight: 900;
  margin-bottom: 4px;
}
.subtitle {
  font-size: 16px;
  color: #555;
}
.menu {
  background: white;
  padding: 16px;
  border-radius: 15px;
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
  padding: 12px;
  border-radius: 10px;
}
select {
  border: 1px solid #aaa;
  background: white;
}
button {
  margin-top: 14px;
  border: 0;
  background: #222;
  color: white;
  font-weight: bold;
  cursor: pointer;
  -webkit-tap-highlight-color: transparent;
}
button:active {
  transform: scale(.98);
}
.task-preview {
  margin-top: 16px;
  padding: 16px;
  border-radius: 12px;
  background: #f0f0f0;
  font-size: 16px;
  line-height: 1.5;
  text-align: left;
  display: none;
}
.task-preview strong {
  font-weight: 900;
}
.game {
  display: none;
  text-align: center;
  padding-top: 10px;
}
.game-task {
  background: white;
  padding: 20px;
  border-radius: 15px;
  box-shadow: 0 2px 9px #0002;
  font-size: 26px;
  line-height: 1.4;
  margin-bottom: 16px;
  text-align: center;
  display: none;
}
.timer-box {
  margin-top: 10px;
  padding: 36px 20px;
  border-radius: 18px;
  background: #222;
  color: white;
}
.timer {
  font-size: 110px;
  line-height: 1;
  font-weight: 900;
  font-variant-numeric: tabular-nums;
}
.timer.warning {
  color: #ffd400;
}
.timer.danger {
  color: #ff4b4b;
}
.status {
  margin-top: 20px;
  padding: 18px;
  border-radius: 15px;
  background: white;
  font-size: 20px;
  font-weight: 900;
  line-height: 1.4;
}
.status.observe {
  color: #0645ad;
}
.status.transition {
  color: #a00000;
  background: #fff1f1;
}
.status.decide {
  color: #a00000;
  background: #fff1f1;
}
.status.finished {
  color: #16832c;
  background: #e8f5e9;
}
.secondary {
  background: white;
  color: #222;
  border: 1px solid #888;
  margin-top: 20px;
  display: none;
}
</style>
</head>
<body>
<div class="app">
  <div class="header">
    <div class="title">TOTAL VERSCHNURRT</div>
    <div class="subtitle">Raum 4</div>
  </div>

  <div class="menu" id="menu">
    <label for="difficulty">Schwierigkeit</label>
    <select id="difficulty">
      <option value="easy">🟢 Leicht (1 Schnur) – 25 Sek.</option>
      <option value="medium">🟡 Mittel (2 Schnüre) – 30 Sek.</option>
      <option value="hard">🟠 Schwer (3 Schnüre) – 35 Sek.</option>
      <option value="veryhard">🔴 Sehr schwer (4 Schnüre) – 40 Sek.</option>
    </select>
    <div class="task-preview" id="taskPreview"></div>
    <button type="button" id="startButton">Runde starten</button>
  </div>

  <div class="game" id="game">
    <div class="game-task" id="gameTask"></div>
    <div class="timer-box">
      <div class="timer" id="timer">0</div>
    </div>
    <div class="status observe" id="status">Zeit läuft …</div>
    <button type="button" class="secondary" id="newRoundButton">Neue Runde</button>
  </div>
</div>

<script>
const times = {
  easy: 25,
  medium: 30,
  hard: 35,
  veryhard: 40
};
const TRANSITION_TIME = 5;
const DECIDE_TIME = 20;

const tasks = {
  easy: [
    { full: "Unter welcher Zahl ist die <strong>rote</strong> Kugel versteckt?<br><br>Verfolge die rote Schnur nur mit den Augen.", short: "<strong>Rot</strong>" },
    { full: "Unter welcher Zahl ist die <strong>orange</strong> Kugel versteckt?<br><br>Verfolge die orange Schnur nur mit den Augen.", short: "<strong>Orange</strong>" },
    { full: "Unter welcher Zahl ist die <strong>grüne</strong> Kugel versteckt?<br><br>Verfolge die grüne Schnur nur mit den Augen.", short: "<strong>Grün</strong>" },
    { full: "Unter welcher Zahl ist die <strong>gelbe</strong> Kugel versteckt?<br><br>Verfolge die gelbe Schnur nur mit den Augen.", short: "<strong>Gelb</strong>" },
    { full: "Unter welcher Zahl ist die <strong>rote</strong> Kugel versteckt?<br><br>Verfolge die rote Schnur nur mit den Augen.", short: "<strong>Rot</strong>" },
    { full: "Unter welcher Zahl ist die <strong>orange</strong> Kugel versteckt?<br><br>Verfolge die orange Schnur nur mit den Augen.", short: "<strong>Orange</strong>" }
  ],
  medium: [
    { full: "Unter welchen Zahlen sind die <strong>rote</strong> und die <strong>orange</strong> Kugel versteckt?<br><br>Verfolge beide Schnüre nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Orange</strong>" },
    { full: "Unter welchen Zahlen sind die <strong>grüne</strong> und die <strong>gelbe</strong> Kugel versteckt?<br><br>Verfolge beide Schnüre nur mit den Augen.", short: "<strong>Grün</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind die <strong>rote</strong> und die <strong>grüne</strong> Kugel versteckt?<br><br>Verfolge beide Schnüre nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Grün</strong>" },
    { full: "Unter welchen Zahlen sind die <strong>orange</strong> und die <strong>gelbe</strong> Kugel versteckt?<br><br>Verfolge beide Schnüre nur mit den Augen.", short: "<strong>Orange</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind die <strong>rote</strong> und die <strong>gelbe</strong> Kugel versteckt?<br><br>Verfolge beide Schnüre nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind die <strong>orange</strong> und die <strong>grüne</strong> Kugel versteckt?<br><br>Verfolge beide Schnüre nur mit den Augen.", short: "<strong>Orange</strong> + <strong>Grün</strong>" }
  ],
  hard: [
    { full: "Unter welchen Zahlen sind die <strong>rote</strong>, die <strong>orange</strong> und die <strong>grüne</strong> Kugel versteckt?<br><br>Verfolge die drei Schnüre nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Orange</strong> + <strong>Grün</strong>" },
    { full: "Unter welchen Zahlen sind die <strong>orange</strong>, die <strong>grüne</strong> und die <strong>gelbe</strong> Kugel versteckt?<br><br>Verfolge die drei Schnüre nur mit den Augen.", short: "<strong>Orange</strong> + <strong>Grün</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind die <strong>rote</strong>, die <strong>grüne</strong> und die <strong>gelbe</strong> Kugel versteckt?<br><br>Verfolge die drei Schnüre nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Grün</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind die <strong>rote</strong>, die <strong>orange</strong> und die <strong>gelbe</strong> Kugel versteckt?<br><br>Verfolge die drei Schnüre nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Orange</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind die <strong>rote</strong>, die <strong>orange</strong> und die <strong>grüne</strong> Kugel versteckt?<br><br>Verfolge die drei Schnüre nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Orange</strong> + <strong>Grün</strong>" },
    { full: "Unter welchen Zahlen sind die <strong>orange</strong>, die <strong>grüne</strong> und die <strong>gelbe</strong> Kugel versteckt?<br><br>Verfolge die drei Schnüre nur mit den Augen.", short: "<strong>Orange</strong> + <strong>Grün</strong> + <strong>Gelb</strong>" }
  ],
  veryhard: [
    { full: "Unter welchen Zahlen sind <strong>alle vier</strong> Kugeln versteckt?<br><br>Verfolge die rote, orange, grüne und gelbe Schnur nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Orange</strong> + <strong>Grün</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind <strong>alle vier</strong> Kugeln versteckt?<br><br>Verfolge die rote, orange, grüne und gelbe Schnur nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Orange</strong> + <strong>Grün</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind <strong>alle vier</strong> Kugeln versteckt?<br><br>Verfolge die rote, orange, grüne und gelbe Schnur nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Orange</strong> + <strong>Grün</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind <strong>alle vier</strong> Kugeln versteckt?<br><br>Verfolge die rote, orange, grüne und gelbe Schnur nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Orange</strong> + <strong>Grün</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind <strong>alle vier</strong> Kugeln versteckt?<br><br>Verfolge die rote, orange, grüne und gelbe Schnur nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Orange</strong> + <strong>Grün</strong> + <strong>Gelb</strong>" },
    { full: "Unter welchen Zahlen sind <strong>alle vier</strong> Kugeln versteckt?<br><br>Verfolge die rote, orange, grüne und gelbe Schnur nur mit den Augen.", short: "<strong>Rot</strong> + <strong>Orange</strong> + <strong>Grün</strong> + <strong>Gelb</strong>" }
  ]
};

const taskIndex = {
  easy: 0,
  medium: 0,
  hard: 0,
  veryhard: 0
};

const menu = document.getElementById("menu");
const game = document.getElementById("game");
const difficulty = document.getElementById("difficulty");
const taskPreview = document.getElementById("taskPreview");
const gameTask = document.getElementById("gameTask");
const startButton = document.getElementById("startButton");
const timer = document.getElementById("timer");
const status = document.getElementById("status");
const newRoundButton = document.getElementById("newRoundButton");

let interval = null;
let currentTask = null;
let currentTime = 25;

function playKlingelton() {
  try {
    const AudioContext = window.AudioContext || window.webkitAudioContext;
    const ctx = new AudioContext();

    const osc1 = ctx.createOscillator();
    const gain1 = ctx.createGain();
    osc1.type = "sine";
    osc1.frequency.value = 880;
    gain1.gain.setValueAtTime(0.0001, ctx.currentTime);
    gain1.gain.exponentialRampToValueAtTime(0.4, ctx.currentTime + 0.02);
    gain1.gain.exponentialRampToValueAtTime(0.0001, ctx.currentTime + 0.35);
    osc1.connect(gain1);
    gain1.connect(ctx.destination);
    osc1.start(ctx.currentTime);
    osc1.stop(ctx.currentTime + 0.35);

    const osc2 = ctx.createOscillator();
    const gain2 = ctx.createGain();
    osc2.type = "sine";
    osc2.frequency.value = 660;
    gain2.gain.setValueAtTime(0.0001, ctx.currentTime + 0.4);
    gain2.gain.exponentialRampToValueAtTime(0.4, ctx.currentTime + 0.42);
    gain2.gain.exponentialRampToValueAtTime(0.0001, ctx.currentTime + 0.75);
    osc2.connect(gain2);
    gain2.connect(ctx.destination);
    osc2.start(ctx.currentTime + 0.4);
    osc2.stop(ctx.currentTime + 0.75);
  } catch (e) {
    console.log("Klingelton konnte nicht abgespielt werden.");
  }
}

function stopTimer() {
  clearInterval(interval);
  interval = null;
}

function startObservationTimer(seconds) {
  stopTimer();
  gameTask.style.display = "block";
  gameTask.innerHTML = currentTask.short;

  let time = seconds;
  timer.textContent = time;
  timer.className = "timer";
  status.className = "status observe";
  status.textContent = "Nur mit den Augen verfolgen!";
  newRoundButton.style.display = "none";

  interval = setInterval(function () {
    time--;
    timer.textContent = time;

    if (time <= 10 && time > 5) {
      timer.classList.add("warning");
    }
    if (time <= 5) {
      timer.classList.remove("warning");
      timer.classList.add("danger");
    }

    if (time <= 0) {
      stopTimer();
      playKlingelton();
      startTransition();
    }
  }, 1000);
}

function startTransition() {
  gameTask.style.display = "none";

  timer.textContent = "–";
  timer.className = "timer";
  status.className = "status transition";
  status.innerHTML =
    "Legt eure gemeinsame Entscheidung<br>" +
    "und Einsprüche auf den Tisch.";

  let wait = TRANSITION_TIME;
  interval = setInterval(function () {
    wait--;
    if (wait <= 0) {
      stopTimer();
      startDecideTimer();
    }
  }, 1000);
}

function startDecideTimer() {
  let time = DECIDE_TIME;
  timer.textContent = time;
  timer.className = "timer danger";
  status.className = "status decide";
  status.innerHTML =
    "Legt eure gemeinsame Entscheidung<br>" +
    "und Einsprüche innerhalb von<br>" +
    "<strong>20 Sekunden</strong> auf den Tisch.";

  interval = setInterval(function () {
    time--;
    timer.textContent = time;

    if (time <= 0) {
      stopTimer();
      playKlingelton();
      timer.textContent = "0";
      status.className = "status finished";
      status.innerHTML =
        "ZEIT ABGELAUFEN<br><br>" +
        "Die Entscheidung und Einsprüche<br>müssen jetzt auf dem Tisch liegen.";
      newRoundButton.style.display = "block";
    }
  }, 1000);
}

function pickAndShowTask() {
  const level = difficulty.value;
  const list = tasks[level];

  currentTask = list[taskIndex[level]];
  currentTime = times[level];
  taskIndex[level] = (taskIndex[level] + 1) % list.length;

  taskPreview.innerHTML =
    currentTask.full +
    "<br><br><strong>" + currentTime + " Sekunden</strong>";
  taskPreview.style.display = "block";
}

difficulty.addEventListener("change", pickAndShowTask);

startButton.addEventListener("click", function () {
  if (!currentTask) pickAndShowTask();
  menu.style.display = "none";
  game.style.display = "block";
  startObservationTimer(currentTime);
});

newRoundButton.addEventListener("click", function () {
  stopTimer();
  game.style.display = "none";
  menu.style.display = "block";
  gameTask.style.display = "none";
  timer.textContent = "0";
  status.textContent = "Zeit läuft …";
  status.className = "status observe";
  newRoundButton.style.display = "none";
  pickAndShowTask();
});

pickAndShowTask();
</script>
</body>
</html>
