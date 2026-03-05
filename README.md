<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Uma Pergunta Importante ❤️</title>

<style>
body{
    font-family: Arial, sans-serif;
    background: #ffdde1;
    text-align: center;
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
}

.container{
    background:white;
    padding:40px;
    border-radius:15px;
    box-shadow:0 10px 30px rgba(0,0,0,0.2);
}

h1{
    margin-bottom:30px;
}

button{
    padding:15px 25px;
    font-size:18px;
    border:none;
    border-radius:10px;
    cursor:pointer;
}

#sim{
    background:#4CAF50;
    color:white;
}

#nao{
    background:#f44336;
    color:white;
    position:absolute;
}
</style>
</head>

<body>

<div class="container">
<h1>Você aceita sair comigo? ❤️ (Não tem como não aceitar) </h1>

<button id="sim" onclick="aceitou()">SIM</button>
<button id="nao">NÃO</button>
</div>

<script>

const nao = document.getElementById("nao");

nao.addEventListener("mouseover", () => {

    const largura = window.innerWidth - 100;
    const altura = window.innerHeight - 100;

    const x = Math.random() * largura;
    const y = Math.random() * altura;

    nao.style.left = x + "px";
    nao.style.top = y + "px";

});

function aceitou(){
    document.body.innerHTML = "<h1 style='font-family:Arial'>Eu sabia!! ❤️😄</h1>";
}

</script>

</body>
</html>
