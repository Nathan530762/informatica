index.html
<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nathan Rodrigues Informática</title>
<style>
body {
    margin:0;
    font-family: Arial, sans-serif;
    background:#f4f4f4;
}
header {
    background:#0a0a23;
    color:white;
    padding:40px 20px;
    text-align:center;
}
header h1 {
    margin:0;
    font-size:32px;
}
header p {
    margin:10px 0;
}
.btn {
    display:inline-block;
    padding:12px 25px;
    background:#25D366;
    color:white;
    text-decoration:none;
    border-radius:5px;
    font-weight:bold;
}
.section {
    padding:40px 20px;
    text-align:center;
}
.promo {
    background:#ffe600;
    padding:20px;
    font-size:20px;
    font-weight:bold;
}
.services div {
    background:white;
    margin:10px auto;
    padding:20px;
    max-width:400px;
    border-radius:8px;
    box-shadow:0 0 10px rgba(0,0,0,0.1);
}
.testimonials {
    background:#fff;
}
footer {
    background:#0a0a23;
    color:white;
    text-align:center;
    padding:20px;
}
.whatsapp-float {
    position:fixed;
    width:60px;
    height:60px;
    bottom:20px;
    right:20px;
    background:#25D366;
    border-radius:50%;
    text-align:center;
    line-height:60px;
    font-size:30px;
    color:white;
    text-decoration:none;
}
</style>
</head>
<body>

<header>
<h1>Nathan Rodrigues Informática</h1>
<p>Seu computador está lento? Nós cuidamos disso para você!</p>
<a class="btn" href="https://wa.me/553195029814" target="_blank">Falar no WhatsApp</a>
</header>

<div class="promo">
🔥 PROMOÇÃO: Formatação + Backup + Drivers + Ativação Windows por apenas R$120 🔥
<p>Oferta válida por tempo limitado!</p>
<p id="countdown"></p>
</div>

<div class="section services">
<h2>Serviços</h2>

<div>
<h3>Formatação Completa</h3>
<p>Instalação limpa e rápida do Windows.</p>
</div>

<div>
<h3>Backup Seguro</h3>
<p>Seus arquivos protegidos antes da formatação.</p>
</div>

<div>
<h3>Instalação de Programas</h3>
<p>Pacote Office, navegadores e programas essenciais.</p>
</div>

<div>
<h3>Limpeza e Otimização</h3>
<p>Seu PC mais rápido e sem travamentos.</p>
</div>

</div>

<div class="section testimonials">
<h2>Depoimentos</h2>

<p>⭐⭐⭐⭐⭐ "Meu computador ficou novo! Super recomendo." - Cliente</p>
<p>⭐⭐⭐⭐⭐ "Atendimento rápido e preço justo!" - Cliente</p>

</div>

<footer>
<p>📞 WhatsApp: (31) 95029-9814</p>
<p>📍 Ouro Branco - MG</p>
</footer>

<a href="https://wa.me/553195029814" class="whatsapp-float" target="_blank">💬</a>

<script>
// Contagem regressiva de 3 dias
var countDownDate = new Date();
countDownDate.setDate(countDownDate.getDate() + 3);

var x = setInterval(function() {
var now = new Date().getTime();
var distance = countDownDate - now;

var days = Math.floor(distance / (1000 * 60 * 60 * 24));
var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));

document.getElementById("countdown").innerHTML =
"⏳ Termina em: " + days + "d " + hours + "h " + minutes + "m ";

if (distance < 0) {
clearInterval(x);
document.getElementById("countdown").innerHTML = "Promoção encerrada";
}
}, 1000);
</script>

</body>
</html>

