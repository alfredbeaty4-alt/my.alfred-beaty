<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Love Test</title>

<style>
* {
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body {
  margin: 0;
  background: #000;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.card {
  width: 90%;
  max-width: 420px;
  background: linear-gradient(180deg, #fff5f8, #ffe6ef);
  border-radius: 30px;
  padding: 25px;
  text-align: center;
  box-shadow: 0 0 20px rgba(255,105,135,.4);
}

h1 {
  color: #ff5c8a;
  margin-bottom: 20px;
  font-weight: 600;
}

input {
  width: 100%;
  padding: 14px;
  margin: 10px 0;
  border-radius: 20px;
  border: none;
  outline: none;
  font-size: 16px;
}

button {
  width: 100%;
  padding: 15px;
  margin-top: 15px;
  border-radius: 25px;
  border: none;
  background: #ff5c8a;
  color: #fff;
  font-size: 17px;
  cursor: pointer;
}

.hidden {
  display: none;
}

.result {
  font-size: 32px;
  color: #ff5c8a;
  margin: 15px 0;
}

.chat {
  background: #ffe0ea;
  padding: 12px;
  border-radius: 18px;
  margin-bottom: 20px;
  display: inline-block;
}

.footer {
  margin-top: 20px;
  font-size: 12px;
  color: #888;
}
</style>
</head>

<body>

<!-- LOVE TEST -->
<div class="card" id="loveTest">
  <h1>Love Test</h1>
  <input id="name1" placeholder="Your name">
  <input id="name2" placeholder="Partner name">
  <button onclick="checkLove()">Check Connection 💖</button>
  <div class="footer">CREATED BY ALFRED BEATY(FREDO)</div>
</div>

<!-- RESULT -->
<div class="card hidden" id="resultPage">
  <h1 id="names"></h1>
  <div class="result" id="percentage"></div>
  <button onclick="openChat()">Talk to AI Girlfriend 🤍</button>
  <div class="footer">CREATED BY ALFRED BEATY(FREDO)</div>
</div>

<!-- AI CHAT -->
<div class="card hidden" id="chatPage">
  <h1>AI Companion</h1>
  <div class="chat" id="chatText">Hi ❤️</div>
  <button onclick="reply()">Reply 💬</button>
  <button onclick="restart()" style="background:#ffc1d4;color:#333;">Restart 🔁</button>
  <div class="footer">CREATED BY ALFRED BEATY(FREDO)</div>
</div>

<script>
let userName = "";

function checkLove() {
  const n1 = document.getElementById("name1").value.trim();
  const n2 = document.getElementById("name2").value.trim();

  if (!n1 || !n2) {
    alert("Please enter both names");
    return;
  }

  userName = n1;
  const love = Math.floor(Math.random() * 21) + 80; // 80–100%

  document.getElementById("loveTest").classList.add("hidden");
  document.getElementById("resultPage").classList.remove("hidden");

  document.getElementById("names").innerText = `${n1} ❤️ ${n2}`;
  document.getElementById("percentage").innerText = love + "%";
}

function openChat() {
  document.getElementById("resultPage").classList.add("hidden");
  document.getElementById("chatPage").classList.remove("hidden");
  document.getElementById("chatText").innerText = `Hi ${userName} 🥺`;
}

function reply() {
  const replies = [
    "I was thinking about you 💕",
    "You make my heart smile 😘",
    "Tell me more about your day ❤️",
    "I feel safe talking to you 🥰"
  ];
  document.getElementById("chatText").innerText =
    replies[Math.floor(Math.random() * replies.length)];
}

function restart() {
  location.reload();
}
</script>

</body>
</html>
