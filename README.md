# Splash-Brasil
Splash
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Splash</title>

<style>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, orange, purple);
    color: white;
    text-align: center;
}

header {
    background: black;
    padding: 15px;
    font-size: 24px;
    font-weight: bold;
}

.container {
    padding: 20px;
}

button {
    padding: 10px 20px;
    margin: 10px;
    border: none;
    border-radius: 8px;
    background: white;
    color: black;
    font-weight: bold;
    cursor: pointer;
}

button:hover {
    background: #ddd;
}

#chatBox {
    position: fixed;
    top: 10%;
    left: 10%;
    width: 80%;
    height: 80%;
    background: black;
    display: none;
    border: 3px solid white;
}

#chatBox iframe {
    width: 100%;
    height: 90%;
    border: none;
}

#closeBtn {
    background: red;
    color: white;
    width: 100%;
}
</style>
</head>

<body>

<header>Splash Brasil</header>

<div class="container">

<p><b>Revival da Nickelodeon sem fins lucrativos</b></p>
<p>Criado em 22 de janeiro de 2026</p>
<p>📺 Entra no ar às vezes (tipo sábados às 11:00 da manhã)</p>

<h2>🔴 AO VIVO</h2>

<iframe src="https://new.opencaster.com/player/embed?user=SplashBR"
width="720" height="360" frameborder="0" allowfullscreen></iframe>

<br>

<button onclick="abrirChat()">💬 Abrir Chat</button>

</div>

<div id="chatBox">
    <button id="closeBtn" onclick="fecharChat()">❌ Fechar</button>
    <iframe src="https://slimetvbrasiloficial.chatango.com"></iframe>
</div>

<script>
function abrirChat() {
    document.getElementById("chatBox").style.display = "block";
}

function fecharChat() {
    document.getElementById("chatBox").style.display = "none";
}
</script>

</body>
</html>
