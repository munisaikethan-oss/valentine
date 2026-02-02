<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Will You Be My Valentine?</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: linear-gradient(#ffd6e8, #fff);
  text-align: center;
  overflow: hidden;
}
.container {
  max-width: 360px;
  margin: 40px auto;
  background: #fff;
  border-radius: 20px;
  padding: 20px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
}
h1 {
  color: #e91e63;
  font-family: cursive;
}
.hearts {
  font-size: 24px;
}
button {
  border: none;
  padding: 12px 24px;
  font-size: 18px;
  border-radius: 30px;
  cursor: pointer;
  margin: 10px;
}
#yes {
  background: #e91e63;
  color: #fff;
}
#no {
  background: #ccc;
  position: absolute;
}
</style>
</head>

<body>
<div class="container">
  <h1>Vinu 💖</h1>
  <p class="hearts">❤️ 💕 ❤️</p>
  <h2>Will you be my Valentine?</h2>
  <p>Choose wisely… 💘</p>

  <button id="yes" onclick="yes()">Yes! 💕</button>
  <button id="no" onmouseover="moveNo()">No 😢</button>
</div>

<script>
function moveNo() {
  const btn = document.getElementById('no');
  btn.style.top = Math.random() * window.innerHeight + 'px';
  btn.style.left = Math.random() * window.innerWidth + 'px';
}

function yes() {
  alert("Good choice ❤️😊");
}
</script>
</body>
</html>
