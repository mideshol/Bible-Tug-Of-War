<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bible Tug of War!</title>
<link href="https://fonts.googleapis.com/css2?family=Fredoka+One&family=Nunito:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
  :root {
    --sky: #87CEEB;
    --grass: #5cb85c;
    --dark-grass: #3d8b3d;
    --sun: #FFD700;
    --cloud: #fff;
    --rope: #c8a45a;
    --rope-dark: #8B6914;
    --team-a: #e74c3c;
    --team-b: #3498db;
    --gold: #f1c40f;
    --correct: #2ecc71;
    --wrong: #e74c3c;
    --panel: rgba(255,255,255,0.92);
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'Nunito', sans-serif;
    background: linear-gradient(180deg, #87CEEB 0%, #b0e0ff 60%, #5cb85c 60%, #3d8b3d 100%);
    min-height: 100vh;
    overflow-x: hidden;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  /* ── Sky decorations ── */
  .sky-deco {
    position: fixed; top: 0; left: 0; width: 100%; height: 58%;
    pointer-events: none; z-index: 0;
  }
  .sun {
    position: absolute; top: 18px; right: 60px;
    width: 70px; height: 70px;
    background: radial-gradient(circle, #ffe066 60%, #FFD700 100%);
    border-radius: 50%;
    box-shadow: 0 0 0 12px rgba(255,215,0,0.18), 0 0 0 24px rgba(255,215,0,0.08);
    animation: pulse-sun 3s ease-in-out infinite;
  }
  @keyframes pulse-sun { 0%,100%{transform:scale(1)} 50%{transform:scale(1.07)} }
  .cloud {
    position: absolute; background: #fff;
    border-radius: 50px;
    opacity: 0.9;
    animation: drift linear infinite;
  }
  .cloud::before, .cloud::after {
    content:''; position:absolute; background:#fff; border-radius:50%;
  }
  .c1{width:90px;height:32px;top:30px;left:-100px;animation-duration:22s}
  .c1::before{width:50px;height:44px;top:-22px;left:12px}
  .c1::after{width:36px;height:36px;top:-16px;left:40px}
  .c2{width:120px;height:36px;top:60px;left:-140px;animation-duration:30s;animation-delay:-10s}
  .c2::before{width:60px;height:50px;top:-26px;left:18px}
  .c2::after{width:44px;height:44px;top:-20px;left:54px}
  .c3{width:70px;height:24px;top:20px;left:-80px;animation-duration:26s;animation-delay:-5s}
  .c3::before{width:38px;height:36px;top:-18px;left:8px}
  .c3::after{width:28px;height:28px;top:-12px;left:32px}
  @keyframes drift {from{transform:translateX(0)} to{transform:translateX(110vw)}}

  /* ── Header ── */
  header {
    position: relative; z-index: 10;
    text-align: center;
    padding: 24px 20px 10px;
  }
  header h1 {
    font-family: 'Fredoka One', cursive;
    font-size: clamp(2rem, 6vw, 3.5rem);
    color: #fff;
    text-shadow: 3px 4px 0 #b85c00, 0 0 30px rgba(255,200,0,0.4);
    letter-spacing: 2px;
  }
  header p {
    color: #fff; font-size: 1rem; font-weight: 700;
    text-shadow: 1px 2px 0 rgba(0,0,0,0.3);
    margin-top: 4px;
  }

  /* ── Scoreboard ── */
  .scoreboard {
    position: relative; z-index: 10;
    display: flex; align-items: center; justify-content: center;
    gap: 12px; margin: 8px 0 0;
  }
  .score-box {
    background: var(--panel);
    border-radius: 16px;
    padding: 8px 20px;
    text-align: center;
    box-shadow: 0 4px 14px rgba(0,0,0,0.15);
    min-width: 100px;
  }
  .score-box .label {
    font-size: 0.75rem; font-weight: 800; text-transform: uppercase; letter-spacing: 1px;
  }
  .score-box .pts {
    font-family: 'Fredoka One', cursive;
    font-size: 2.2rem; line-height: 1;
  }
  .team-a .label { color: var(--team-a); }
  .team-a .pts   { color: var(--team-a); }
  .team-b .label { color: var(--team-b); }
  .team-b .pts   { color: var(--team-b); }
  .vs-badge {
    font-family: 'Fredoka One', cursive;
    font-size: 1.4rem; color: #fff;
    text-shadow: 2px 2px 0 rgba(0,0,0,0.25);
  }

  /* ── Tug of War Scene ── */
  .tug-scene {
    position: relative; z-index: 10;
    width: min(700px, 96vw);
    height: 130px;
    margin: 6px auto 0;
  }

  /* flag in the middle */
  .mud-line {
    position: absolute;
    left: 50%; top: 50%; transform: translate(-50%, -50%);
    width: 6px; height: 70px;
    background: #8B4513;
    border-radius: 3px;
  }
  .flag {
    position: absolute;
    top: -4px; left: 6px;
    width: 22px; height: 16px;
    background: #e74c3c;
    clip-path: polygon(0 0, 100% 50%, 0 100%);
    animation: wave-flag 0.6s ease-in-out infinite alternate;
  }
  @keyframes wave-flag { from{transform:skewY(-4deg)} to{transform:skewY(4deg)} }

  /* rope */
  .rope-wrap {
    position: absolute;
    top: 50%; left: 0; right: 0;
    transform: translateY(-50%);
    height: 22px;
    display: flex; align-items: center;
  }
  .rope {
    height: 14px;
    flex: 1;
    background: repeating-linear-gradient(
      90deg,
      var(--rope) 0px, var(--rope) 10px,
      var(--rope-dark) 10px, var(--rope-dark) 20px
    );
    border-radius: 7px;
    position: relative;
    transition: margin 0.6s cubic-bezier(.34,1.56,.64,1);
    box-shadow: 0 3px 0 rgba(0,0,0,0.2);
  }

  /* stick figures */
  .team-group {
    position: absolute;
    bottom: 0;
    display: flex;
    align-items: flex-end;
    gap: 2px;
  }
  .team-a-group { left: 0; flex-direction: row; }
  .team-b-group { right: 0; flex-direction: row-reverse; }

  .figure {
    display: flex; flex-direction: column; align-items: center;
    width: 36px;
    position: relative;
    transition: transform 0.5s cubic-bezier(.34,1.56,.64,1);
  }
  .figure .head {
    width: 18px; height: 18px; border-radius: 50%;
    border: 3px solid currentColor;
    background: #FFDAB9;
    margin-bottom: 2px;
  }
  .figure .body {
    width: 3px; height: 28px;
    background: currentColor;
    position: relative;
  }
  .figure .arms {
    position: absolute;
    top: 6px; left: 50%; transform: translateX(-50%);
    width: 26px; height: 3px;
    background: currentColor;
  }
  .figure .legs {
    display: flex; gap: 6px;
    margin-top: 2px;
  }
  .figure .leg {
    width: 3px; height: 22px;
    background: currentColor;
    border-radius: 0 0 2px 2px;
    transform-origin: top;
  }
  .figure.team-a { color: var(--team-a); }
  .figure.team-b { color: var(--team-b); }

  /* lean animations */
  .figure.team-a { transform: rotate(-12deg); }
  .figure.team-b { transform: rotate(12deg); }
  .figure.winning { animation: heave 0.4s ease-in-out infinite alternate; }
  .figure.team-a.winning { animation-name: heave-a; }
  .figure.team-b.winning { animation-name: heave-b; }
  @keyframes heave-a { from{transform:rotate(-14deg) translateX(0)} to{transform:rotate(-8deg) translateX(-3px)} }
  @keyframes heave-b { from{transform:rotate(14deg) translateX(0)} to{transform:rotate(8deg) translateX(3px)} }

  /* ── Progress bar under scene ── */
  .progress-bar-wrap {
    position: relative; z-index: 10;
    width: min(700px, 94vw);
    margin: 4px auto 0;
    background: rgba(0,0,0,0.15);
    border-radius: 20px; height: 20px;
    overflow: hidden;
    box-shadow: inset 0 2px 4px rgba(0,0,0,0.2);
  }
  .progress-fill {
    height: 100%; border-radius: 20px;
    background: linear-gradient(90deg, var(--team-a) 0%, var(--team-b) 100%);
    transition: width 0.6s cubic-bezier(.34,1.56,.64,1);
    position: relative;
  }
  .progress-fill::after {
    content:'';
    position: absolute; right: 0; top: 0;
    width: 4px; height: 100%;
    background: rgba(255,255,255,0.5);
    border-radius: 0 20px 20px 0;
  }
  .progress-center {
    position: absolute; top: 0; left: 50%;
    transform: translateX(-50%);
    height: 100%; width: 3px;
    background: #fff; opacity: 0.5;
  }

  /* ── Question Panel ── */
  .question-panel {
    position: relative; z-index: 10;
    background: var(--panel);
    border-radius: 24px;
    padding: 22px 28px 20px;
    margin: 14px auto 0;
    width: min(680px, 94vw);
    box-shadow: 0 8px 32px rgba(0,0,0,0.18);
    border: 3px solid rgba(255,255,255,0.8);
  }
  .q-meta {
    display: flex; align-items: center; gap: 10px;
    margin-bottom: 10px;
  }
  .q-badge {
    font-family: 'Fredoka One', cursive;
    font-size: 0.8rem;
    padding: 3px 10px;
    border-radius: 30px;
    color: #fff;
  }
  .q-badge.easy   { background: #2ecc71; }
  .q-badge.medium { background: #f39c12; }
  .q-badge.hard   { background: #e74c3c; }
  .q-num { font-size: 0.8rem; color: #888; font-weight: 700; }

  .question-text {
    font-family: 'Fredoka One', cursive;
    font-size: clamp(1.1rem, 3vw, 1.5rem);
    color: #2c3e50;
    margin-bottom: 16px;
    line-height: 1.35;
  }
  .answers-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
  }
  .answer-btn {
    padding: 12px 14px;
    border: 3px solid #e0e0e0;
    border-radius: 14px;
    background: #fff;
    font-family: 'Nunito', sans-serif;
    font-size: 1rem; font-weight: 800;
    color: #2c3e50;
    cursor: pointer;
    transition: all 0.15s;
    text-align: left;
    line-height: 1.3;
  }
  .answer-btn:hover:not(:disabled) {
    border-color: #3498db;
    background: #eaf4fd;
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(52,152,219,0.25);
  }
  .answer-btn.correct {
    border-color: var(--correct); background: #d5f5e3;
    animation: pop 0.3s ease;
  }
  .answer-btn.wrong {
    border-color: var(--wrong); background: #fde8e8;
    animation: shake 0.4s ease;
  }
  @keyframes pop { 0%{transform:scale(0.95)} 60%{transform:scale(1.06)} 100%{transform:scale(1)} }
  @keyframes shake { 0%,100%{transform:translateX(0)} 25%{transform:translateX(-6px)} 75%{transform:translateX(6px)} }

  .feedback {
    margin-top: 14px;
    padding: 10px 16px;
    border-radius: 12px;
    font-weight: 800; font-size: 1.05rem;
    display: none;
    align-items: center; gap: 8px;
  }
  .feedback.show { display: flex; }
  .feedback.correct { background: #d5f5e3; color: #1a7a45; }
  .feedback.wrong   { background: #fde8e8; color: #c0392b; }

  .next-btn {
    margin-top: 14px;
    padding: 12px 32px;
    font-family: 'Fredoka One', cursive;
    font-size: 1.2rem;
    color: #fff;
    background: linear-gradient(135deg, #f1c40f, #e67e22);
    border: none; border-radius: 30px;
    cursor: pointer;
    box-shadow: 0 4px 0 #b7770d, 0 6px 16px rgba(241,196,15,0.4);
    transition: all 0.15s;
    display: none;
  }
  .next-btn:hover { transform: translateY(-2px); box-shadow: 0 6px 0 #b7770d, 0 10px 20px rgba(241,196,15,0.4); }
  .next-btn:active { transform: translateY(2px); box-shadow: 0 2px 0 #b7770d; }
  .next-btn.show { display: inline-block; }

  /* ── Turn indicator ── */
  .turn-indicator {
    text-align: center;
    font-family: 'Fredoka One', cursive;
    font-size: 1.1rem;
    margin-bottom: 12px;
    padding: 6px 18px;
    border-radius: 20px;
    display: inline-block;
  }
  .turn-a { background: #fde8e8; color: var(--team-a); }
  .turn-b { background: #eaf4fd; color: var(--team-b); }

  /* ── Win Screen ── */
  .win-screen {
    display: none;
    position: fixed; inset: 0; z-index: 100;
    background: rgba(0,0,0,0.55);
    align-items: center; justify-content: center;
    flex-direction: column;
  }
  .win-screen.show { display: flex; }
  .win-card {
    background: #fff;
    border-radius: 32px;
    padding: 40px 50px;
    text-align: center;
    box-shadow: 0 20px 60px rgba(0,0,0,0.35);
    animation: zoom-in 0.5s cubic-bezier(.34,1.56,.64,1);
    max-width: 420px; width: 90%;
  }
  @keyframes zoom-in { from{transform:scale(0.5);opacity:0} to{transform:scale(1);opacity:1} }
  .win-emoji { font-size: 4rem; }
  .win-title {
    font-family: 'Fredoka One', cursive;
    font-size: 2.2rem;
    margin: 10px 0 4px;
  }
  .win-sub { font-size: 1rem; color: #555; font-weight: 700; margin-bottom: 18px; }
  .confetti-wrap {
    position: fixed; inset: 0; z-index: 99; pointer-events: none;
  }
  .confetti-piece {
    position: absolute;
    top: -10px;
    width: 10px; height: 14px;
    border-radius: 2px;
    animation: fall linear forwards;
  }
  @keyframes fall {
    0%   { transform: translateY(0) rotate(0deg) translateX(0); opacity: 1; }
    100% { transform: translateY(110vh) rotate(720deg) translateX(var(--drift)); opacity: 0; }
  }
  .play-again-btn {
    padding: 14px 36px;
    font-family: 'Fredoka One', cursive;
    font-size: 1.4rem;
    color: #fff;
    background: linear-gradient(135deg, #2ecc71, #27ae60);
    border: none; border-radius: 30px;
    cursor: pointer;
    box-shadow: 0 4px 0 #1a7a45;
    transition: all 0.15s;
  }
  .play-again-btn:hover { transform: translateY(-2px); }

  /* ── Setup Screen ── */
  .setup-screen {
    position: fixed; inset: 0; z-index: 200;
    background: linear-gradient(180deg, #87CEEB 0%, #b0e0ff 60%, #5cb85c 60%, #3d8b3d 100%);
    display: flex; align-items: center; justify-content: center;
  }
  .setup-card {
    background: rgba(255,255,255,0.95);
    border-radius: 30px;
    padding: 36px 40px;
    text-align: center;
    box-shadow: 0 10px 40px rgba(0,0,0,0.2);
    max-width: 440px; width: 92%;
    animation: zoom-in 0.5s ease;
  }
  .setup-card h2 {
    font-family: 'Fredoka One', cursive;
    font-size: 2rem; color: #2c3e50;
    margin-bottom: 6px;
  }
  .setup-card p { color: #555; font-weight: 700; margin-bottom: 22px; }
  .name-input-row {
    display: flex; flex-direction: column; gap: 12px; margin-bottom: 20px;
  }
  .name-input {
    padding: 12px 18px;
    border-radius: 14px;
    border: 3px solid #e0e0e0;
    font-family: 'Nunito', sans-serif;
    font-size: 1.05rem; font-weight: 700;
    outline: none; transition: border-color 0.2s;
  }
  .name-input:focus { border-color: #3498db; }
  .name-input.team-a-input:focus { border-color: var(--team-a); }
  .name-input.team-b-input:focus { border-color: var(--team-b); }
  .start-btn {
    padding: 14px 44px;
    font-family: 'Fredoka One', cursive;
    font-size: 1.4rem; color: #fff;
    background: linear-gradient(135deg, #e74c3c, #c0392b);
    border: none; border-radius: 30px;
    cursor: pointer;
    box-shadow: 0 4px 0 #922b21;
    transition: all 0.15s;
  }
  .start-btn:hover { transform: translateY(-2px); }

  @media (max-width: 480px) {
    .answers-grid { grid-template-columns: 1fr; }
    .question-panel { padding: 16px 16px 14px; }
  }
</style>
</head>
<body>

<!-- Sky decorations -->
<div class="sky-deco">
  <div class="sun"></div>
  <div class="cloud c1"></div>
  <div class="cloud c2"></div>
  <div class="cloud c3"></div>
</div>

<!-- Setup Screen -->
<div class="setup-screen" id="setupScreen">
  <div class="setup-card">
    <div style="font-size:2.5rem;margin-bottom:4px">📖⚡</div>
    <h2>Bible Tug of War!</h2>
    <p>Two teams answer Bible questions.<br>Pull the rope to win! 🏆</p>
    <div class="name-input-row">
      <input class="name-input team-a-input" id="teamAName" placeholder="🔴 Team A Name (e.g. Lions)" maxlength="16">
      <input class="name-input team-b-input" id="teamBName" placeholder="🔵 Team B Name (e.g. Eagles)" maxlength="16">
    </div>
    <button class="start-btn" onclick="startGame()">Let's Go! 🎉</button>
  </div>
</div>

<!-- Game UI -->
<header>
  <h1>📖 Bible Tug of War!</h1>
  <p>Answer correctly to pull the rope! 💪</p>
</header>

<div class="scoreboard">
  <div class="score-box team-a">
    <div class="label" id="labelA">Team A</div>
    <div class="pts" id="scoreA">0</div>
  </div>
  <div class="vs-badge">VS</div>
  <div class="score-box team-b">
    <div class="label" id="labelB">Team B</div>
    <div class="pts" id="scoreB">0</div>
  </div>
</div>

<!-- Tug of War Scene -->
<div class="tug-scene">
  <!-- Team A figures (left) -->
  <div class="team-group team-a-group" id="teamAFigs"></div>

  <!-- Rope -->
  <div class="rope-wrap">
    <div class="rope" id="ropeEl"></div>
  </div>

  <!-- Center flag -->
  <div class="mud-line" id="mudLine">
    <div class="flag"></div>
  </div>

  <!-- Team B figures (right) -->
  <div class="team-group team-b-group" id="teamBFigs"></div>
</div>

<!-- Progress bar -->
<div class="progress-bar-wrap">
  <div class="progress-fill" id="progressFill" style="width:50%"></div>
  <div class="progress-center"></div>
</div>

<!-- Question Panel -->
<div class="question-panel">
  <div style="text-align:center; margin-bottom:8px">
    <span class="turn-indicator" id="turnIndicator">Team A's Turn</span>
  </div>
  <div class="q-meta">
    <span class="q-badge" id="diffBadge">Easy</span>
    <span class="q-num" id="qNum">Question 1 of 10</span>
  </div>
  <div class="question-text" id="questionText">Loading...</div>
  <div class="answers-grid" id="answersGrid"></div>
  <div class="feedback" id="feedback"></div>
  <button class="next-btn" id="nextBtn" onclick="nextQuestion()">Next Question ➡️</button>
</div>

<!-- Win Screen -->
<div class="win-screen" id="winScreen">
  <div class="confetti-wrap" id="confettiWrap"></div>
  <div class="win-card">
    <div class="win-emoji" id="winEmoji">🏆</div>
    <div class="win-title" id="winTitle">Team A Wins!</div>
    <div class="win-sub" id="winSub">Amazing Bible knowledge! God is pleased! 🌟</div>
    <div style="margin-bottom:16px; font-size:0.95rem; color:#777; font-weight:700" id="winStats"></div>
    <button class="play-again-btn" onclick="resetGame()">Play Again! 🎉</button>
  </div>
</div>

<script>
const QUESTIONS = [
  // ── EASY (20 questions) ──
  { q:"Who built the ark to survive the great flood?", a:["Noah","Moses","Abraham","David"], c:0, diff:"easy" },
  { q:"How many days did it take God to create the world?", a:["7 days","5 days","10 days","3 days"], c:0, diff:"easy" },
  { q:"What giant did David defeat with a sling and stone?", a:["Goliath","Samson","Pharaoh","Esau"], c:0, diff:"easy" },
  { q:"In which garden did Adam and Eve live?", a:["Garden of Eden","Garden of Gethsemane","Garden of Olives","Garden of Bethlehem"], c:0, diff:"easy" },
  { q:"How many disciples did Jesus choose?", a:["12","10","7","15"], c:0, diff:"easy" },
  { q:"What food did God send from heaven to feed Israel in the desert?", a:["Manna","Bread","Fish","Fruit"], c:0, diff:"easy" },
  { q:"What is the first book of the Bible?", a:["Genesis","Exodus","Matthew","Psalms"], c:0, diff:"easy" },
  { q:"Who was swallowed by a big fish?", a:["Jonah","Elijah","Paul","Peter"], c:0, diff:"easy" },
  { q:"What is the last book of the Bible?", a:["Revelation","Acts","Hebrews","Jude"], c:0, diff:"easy" },
  { q:"Jesus was born in which city?", a:["Bethlehem","Nazareth","Jerusalem","Jericho"], c:0, diff:"easy" },
  { q:"Who was the first man God created?", a:["Adam","Noah","Abraham","Moses"], c:0, diff:"easy" },
  { q:"What did Jesus ride when he entered Jerusalem?", a:["A donkey","A horse","A camel","A chariot"], c:0, diff:"easy" },
  { q:"How many commandments did God give Moses?", a:["10","7","12","5"], c:0, diff:"easy" },
  { q:"Who was Jesus' earthly father?", a:["Joseph","John","James","Zechariah"], c:0, diff:"easy" },
  { q:"What were the two people God created first?", a:["Adam and Eve","Cain and Abel","Abraham and Sarah","Moses and Aaron"], c:0, diff:"easy" },
  { q:"Who is known as the 'Good Shepherd' in the Bible?", a:["Jesus","David","Moses","Abraham"], c:0, diff:"easy" },
  { q:"What animal talked to Balaam in the Bible?", a:["A donkey","A serpent","A lion","A dove"], c:0, diff:"easy" },
  { q:"Which sea did Moses part with his staff?", a:["The Red Sea","The Dead Sea","The Sea of Galilee","The Jordan River"], c:0, diff:"easy" },
  { q:"What did God use to create light on the first day?", a:["His word","The sun","Fire","Lightning"], c:0, diff:"easy" },
  { q:"On what day did God rest after creating the world?", a:["The 7th day","The 6th day","The 5th day","The 1st day"], c:0, diff:"easy" },

  // ── MEDIUM (20 questions) ──
  { q:"What were the stone tablets Moses received called?", a:["The Ten Commandments","The Beatitudes","The Proverbs","The Psalms"], c:0, diff:"medium" },
  { q:"In which river was Jesus baptized?", a:["Jordan River","Nile River","Euphrates River","Sea of Galilee"], c:0, diff:"medium" },
  { q:"Who was sold into slavery by his brothers?", a:["Joseph","Benjamin","Isaac","Jacob"], c:0, diff:"medium" },
  { q:"What did Jesus turn water into at a wedding?", a:["Wine","Juice","Milk","Oil"], c:0, diff:"medium" },
  { q:"Who was the mother of Jesus?", a:["Mary","Martha","Elizabeth","Ruth"], c:0, diff:"medium" },
  { q:"How many days was Jesus in the tomb before rising?", a:["3 days","2 days","7 days","1 day"], c:0, diff:"medium" },
  { q:"Which king asked God for wisdom instead of riches?", a:["Solomon","David","Saul","Herod"], c:0, diff:"medium" },
  { q:"Who baptized Jesus?", a:["John the Baptist","Peter","Andrew","Philip"], c:0, diff:"medium" },
  { q:"What was the name of the garden where Jesus prayed before his arrest?", a:["Gethsemane","Eden","Olives","Nazareth"], c:0, diff:"medium" },
  { q:"Who was thrown into the lions' den but survived?", a:["Daniel","Shadrach","Elijah","Paul"], c:0, diff:"medium" },
  { q:"How many sons did Jacob have?", a:["12","10","7","9"], c:0, diff:"medium" },
  { q:"Who was the first king of Israel?", a:["Saul","David","Solomon","Samuel"], c:0, diff:"medium" },
  { q:"What did Jesus feed 5,000 people with?", a:["5 loaves and 2 fish","3 loaves and 5 fish","7 loaves and 1 fish","2 loaves and 7 fish"], c:0, diff:"medium" },
  { q:"Who was Ruth's mother-in-law?", a:["Naomi","Miriam","Deborah","Hannah"], c:0, diff:"medium" },
  { q:"Which disciple denied Jesus three times?", a:["Peter","Judas","Thomas","Andrew"], c:0, diff:"medium" },
  { q:"What were the three young men thrown into for not bowing to the king's statue?", a:["A fiery furnace","A lions' den","A pit","The sea"], c:0, diff:"medium" },
  { q:"Who was the oldest person in the Bible?", a:["Methuselah","Noah","Abraham","Adam"], c:0, diff:"medium" },
  { q:"In what book of the Bible is the story of creation found?", a:["Genesis","Exodus","Numbers","Leviticus"], c:0, diff:"medium" },
  { q:"How many plagues did God send on Egypt?", a:["10","7","5","12"], c:0, diff:"medium" },
  { q:"Who was the prophet that was taken to heaven in a whirlwind?", a:["Elijah","Elisha","Isaiah","Ezekiel"], c:0, diff:"medium" },

  // ── HARD (10 questions) ──
  { q:"How many books are in the entire Bible?", a:["66","39","27","73"], c:0, diff:"hard" },
  { q:"Who wrote most of the Psalms?", a:["David","Moses","Solomon","Isaiah"], c:0, diff:"hard" },
  { q:"Who climbed a tree to see Jesus passing by?", a:["Zacchaeus","Matthew","Andrew","Bartimaeus"], c:0, diff:"hard" },
  { q:"What were the names of the first two brothers in the Bible?", a:["Cain & Abel","Jacob & Esau","Peter & Andrew","James & John"], c:0, diff:"hard" },
  { q:"How many books are in the New Testament?", a:["27","39","66","12"], c:0, diff:"hard" },
  { q:"Who was the high priest that questioned Jesus before his crucifixion?", a:["Caiaphas","Annas","Ananias","Zechariah"], c:0, diff:"hard" },
  { q:"What is the shortest verse in the Bible?", a:["Jesus wept","God is love","Amen","Fear not"], c:0, diff:"hard" },
  { q:"How many years did the Israelites wander in the wilderness?", a:["40 years","20 years","10 years","50 years"], c:0, diff:"hard" },
  { q:"What book comes right after the book of Job?", a:["Psalms","Proverbs","Isaiah","Ecclesiastes"], c:0, diff:"hard" },
  { q:"Who wrote the book of Revelation?", a:["John","Paul","Peter","James"], c:0, diff:"hard" },
];

// Game State
let teamAName = "Team A", teamBName = "Team B";
let scoreA = 0, scoreB = 0;
let ropePosition = 0; // -4 to +4, positive = team B winning
const WIN_THRESHOLD = 4;
let currentQ = 0;
let currentTeam = 'A'; // 'A' or 'B'
let questions = [];
let answered = false;

function shuffle(arr) {
  for (let i = arr.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [arr[i], arr[j]] = [arr[j], arr[i]];
  }
  return arr;
}

function buildFigures() {
  const aDiv = document.getElementById('teamAFigs');
  const bDiv = document.getElementById('teamBFigs');
  aDiv.innerHTML = ''; bDiv.innerHTML = '';

  for (let i = 0; i < 3; i++) {
    aDiv.innerHTML += `<div class="figure team-a" id="figA${i}">
      <div class="head"></div>
      <div class="body"><div class="arms"></div></div>
      <div class="legs"><div class="leg"></div><div class="leg"></div></div>
    </div>`;
    bDiv.innerHTML += `<div class="figure team-b" id="figB${i}">
      <div class="head"></div>
      <div class="body"><div class="arms"></div></div>
      <div class="legs"><div class="leg"></div><div class="leg"></div></div>
    </div>`;
  }
}

function updateRopeScene() {
  // ropePosition: -4 = team A winning, +4 = team B winning
  // Shift the mud-line (flag) and compress rope
  const scene = document.querySelector('.tug-scene');
  const sceneW = scene.offsetWidth;
  const center = sceneW / 2;

  // Move flag: max 30% shift
  const flagShift = (ropePosition / WIN_THRESHOLD) * (sceneW * 0.22);
  const mudLine = document.getElementById('mudLine');
  mudLine.style.left = `calc(50% + ${flagShift}px)`;

  // Update progress bar (50% center, left = team A, right = team B)
  const pct = 50 + (ropePosition / WIN_THRESHOLD) * 40;
  document.getElementById('progressFill').style.width = pct + '%';

  // Highlight winning figures
  for (let i = 0; i < 3; i++) {
    const fa = document.getElementById('figA'+i);
    const fb = document.getElementById('figB'+i);
    if (!fa || !fb) continue;
    fa.classList.remove('winning'); fb.classList.remove('winning');
    if (ropePosition < 0) fa.classList.add('winning');
    if (ropePosition > 0) fb.classList.add('winning');
  }
}

function startGame() {
  const aInput = document.getElementById('teamAName').value.trim();
  const bInput = document.getElementById('teamBName').value.trim();
  teamAName = aInput || 'Team A';
  teamBName = aInput ? (bInput || 'Team B') : 'Team B';
  if (aInput) teamBName = bInput || 'Team B';

  document.getElementById('labelA').textContent = teamAName;
  document.getElementById('labelB').textContent = teamBName;
  document.getElementById('setupScreen').style.display = 'none';

  // Shuffle and pick 10 questions
  questions = shuffle([...QUESTIONS]).slice(0, 10);
  currentQ = 0; scoreA = 0; scoreB = 0; ropePosition = 0; answered = false;
  currentTeam = 'A';

  buildFigures();
  updateRopeScene();
  renderQuestion();
}

function renderQuestion() {
  const q = questions[currentQ];
  document.getElementById('qNum').textContent = `Question ${currentQ+1} of ${questions.length}`;
  
  const badge = document.getElementById('diffBadge');
  badge.textContent = q.diff.charAt(0).toUpperCase() + q.diff.slice(1);
  badge.className = `q-badge ${q.diff}`;

  document.getElementById('questionText').textContent = q.q;
  document.getElementById('feedback').className = 'feedback';
  document.getElementById('nextBtn').className = 'next-btn';
  answered = false;

  // Update turn indicator
  const ti = document.getElementById('turnIndicator');
  if (currentTeam === 'A') {
    ti.textContent = `${teamAName}'s Turn 🔴`;
    ti.className = 'turn-indicator turn-a';
  } else {
    ti.textContent = `${teamBName}'s Turn 🔵`;
    ti.className = 'turn-indicator turn-b';
  }

  // Shuffle answer options
  const opts = q.a.map((text, i) => ({ text, orig: i }));
  shuffle(opts);
  const correctNewIdx = opts.findIndex(o => o.orig === q.c);

  const grid = document.getElementById('answersGrid');
  grid.innerHTML = '';
  opts.forEach((opt, i) => {
    const btn = document.createElement('button');
    btn.className = 'answer-btn';
    btn.textContent = opt.text;
    btn.onclick = () => checkAnswer(i, correctNewIdx, btn, opts.length);
    grid.appendChild(btn);
  });

  updateScoreboard();
}

function checkAnswer(chosen, correct, btn, total) {
  if (answered) return;
  answered = true;

  const btns = document.querySelectorAll('.answer-btn');
  btns.forEach(b => b.disabled = true);
  btns[correct].classList.add('correct');

  const fb = document.getElementById('feedback');
  if (chosen === correct) {
    btn.classList.add('correct');
    fb.className = 'feedback correct show';
    fb.innerHTML = '✅ ' + getCorrectMsg();
    if (currentTeam === 'A') { scoreA++; ropePosition--; }
    else { scoreB++; ropePosition++; }
    updateRopeScene();
    if (Math.abs(ropePosition) >= WIN_THRESHOLD) {
      setTimeout(showWin, 600);
      return;
    }
  } else {
    btn.classList.add('wrong');
    fb.className = 'feedback wrong show';
    fb.innerHTML = '❌ ' + getWrongMsg() + ' The answer was: <b>' + questions[currentQ].a[questions[currentQ].c] + '</b>';
  }

  updateScoreboard();
  document.getElementById('nextBtn').className = 'next-btn show';
}

function getCorrectMsg() {
  const msgs = ["Amazing! 🌟","You got it! 🎉","Fantastic! ⭐","Bible genius! 📖","That's right! 🙌"];
  return msgs[Math.floor(Math.random()*msgs.length)];
}
function getWrongMsg() {
  const msgs = ["Not quite!","Good try!","Almost!","Keep going!"];
  return msgs[Math.floor(Math.random()*msgs.length)];
}

function nextQuestion() {
  currentQ++;
  if (currentQ >= questions.length) {
    showWin();
    return;
  }
  currentTeam = currentTeam === 'A' ? 'B' : 'A';
  renderQuestion();
}

function updateScoreboard() {
  document.getElementById('scoreA').textContent = scoreA;
  document.getElementById('scoreB').textContent = scoreB;
}

function showWin() {
  let winner = '', emoji = '', sub = '';
  if (ropePosition <= -WIN_THRESHOLD || (scoreA > scoreB && currentQ >= questions.length-1)) {
    winner = teamAName;
    emoji = '🏆🔴';
    sub = `${teamAName} pulled the rope all the way! Incredible Bible knowledge!`;
  } else if (ropePosition >= WIN_THRESHOLD || (scoreB > scoreA && currentQ >= questions.length-1)) {
    winner = teamBName;
    emoji = '🏆🔵';
    sub = `${teamBName} pulled the rope all the way! Incredible Bible knowledge!`;
  } else {
    winner = "It's a Tie!";
    emoji = '🤝';
    sub = "Both teams know their Bible really well! Great game!";
  }

  document.getElementById('winEmoji').textContent = emoji;
  document.getElementById('winTitle').textContent = `${winner} Wins!`;
  document.getElementById('winSub').textContent = sub;
  document.getElementById('winStats').textContent = `${teamAName}: ${scoreA} pts  •  ${teamBName}: ${scoreB} pts`;
  document.getElementById('winScreen').className = 'win-screen show';
  launchConfetti();
}

function launchConfetti() {
  const wrap = document.getElementById('confettiWrap');
  wrap.innerHTML = '';
  const colors = ['#e74c3c','#3498db','#2ecc71','#f1c40f','#9b59b6','#e67e22','#1abc9c'];
  for (let i = 0; i < 80; i++) {
    const el = document.createElement('div');
    el.className = 'confetti-piece';
    const color = colors[Math.floor(Math.random()*colors.length)];
    const left = Math.random() * 100;
    const delay = Math.random() * 2;
    const dur = 2.5 + Math.random() * 2;
    const drift = (Math.random()-0.5) * 200;
    el.style.cssText = `left:${left}vw; background:${color}; animation-duration:${dur}s; animation-delay:${delay}s; --drift:${drift}px; transform:rotate(${Math.random()*360}deg)`;
    wrap.appendChild(el);
  }
}

function resetGame() {
  document.getElementById('winScreen').className = 'win-screen';
  document.getElementById('confettiWrap').innerHTML = '';
  document.getElementById('setupScreen').style.display = 'flex';
  document.getElementById('teamAName').value = '';
  document.getElementById('teamBName').value = '';
}
</script>
</body>
</html>
