<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Poema e Música - Boi Garantido</title>

<style>
  body {
    font-family: Arial, sans-serif;
    background: #fff0f0;
    color: #3b0000;
    padding: 2rem;
    max-width: 700px;
    margin: auto;
    text-align: left;
  }
  h1 {
    text-align: center;
    color: #c30000;
  }
  .contador {
    font-size: 1.3rem;
    color: #b30000;
    text-align: center;
    margin: 1rem 0;
  }
  .mensagem p {
    line-height: 1.7;
    margin-bottom: 1rem;
  }
  .qr-code {
    text-align: center;
    margin: 2rem 0;
  }
  iframe {
    display: block;
    margin: 0 auto 2rem auto;
    border-radius: 10px;
  }
</style>

</head>
<body>

<h1>🐂 Boi Garantido foi o sinal</h1>

<div class="contador" id="diasContador">Carregando contador...</div>

<div class="mensagem">
  <p>🐂 Boi Garantido foi o sinal.</p>

  <p>No meio das cores, dos batuques e dos gritos de festa,<br />
  ali estava ela — pulando, cantando, sorrindo como se o mundo fosse leve demais pro tanto de beleza que ela carregava.<br />
  Era dia 06 de junho, mas o tempo parou.</p>

  <p>E naquele instante,<br />
  no calor da multidão, entre o vermelho do boi e o ritmo que ecoava no peito,<br />
  meu olhar se prendeu ao dela — e algo em mim acordou.</p>

  <p>Não sei se foi o jeito que ela dançava,<br />
  ou a forma que os olhos dela brilhavam mais do que todas as luzes do festival.<br />
  Só sei que a partir dali, nada foi igual.</p>

  <p>Aquela bela moça que cantava como quem vive o momento sem medo,<br />
  me encantou num nível que nem sei explicar.<br />
  Foi mais que interesse.<br />
  Foi conexão. Foi paz. Foi bagunça boa por dentro.</p>

  <p>Hoje, ela tem mais do que meu olhar.<br />
  Tem meu coração.<br />
  Tem minhas ideias embaralhadas quando fala comigo.<br />
  Tem meu silêncio quando fico pensando nela, mesmo sem dizer nada.</p>

  <p>Ela talvez nem saiba o quanto já mora em mim —<br />
  mesmo com receios, mesmo com pausas, mesmo com dúvidas.<br />
  Mas o que eu sinto é simples:<br />
  quando ela sorri, meu mundo desacelera.<br />
  E tudo o que era plano, ficou desejo.</p>

  <p>Se um dia isso virar amor vivido, o boi garantido vai ser nosso padrinho.<br />
  Se não, que ela leve com ela o melhor de mim —<br />
  porque desde aquele 06 de junho,<br />
  eu só sei ser verdadeiro com o que senti.</p>
</div>

<iframe width="300" height="169" src="https://www.youtube.com/embed/qxsTuP76JA4" title="Estandarte do Amor - Garantido" frameborder="0" allowfullscreen></iframe>

<div class="qr-code" id="qrcode"></div>

<script src="https://cdn.jsdelivr.net/npm/qrcode@1.5.1/build/qrcode.min.js"></script>
<script>
  // Atualiza o contador de dias desde 06/06/2025
  function atualizarContador() {
    const inicio = new Date("2025-06-06T00:00:00");
    const hoje = new Date();
    const diffTempo = hoje - inicio;
    const dias = Math.floor(diffTempo / (1000 * 60 * 60 * 24));
    document.getElementById("diasContador").innerText = `Já faz ${dias} dias desde o dia em que nos conhecemos ❤️`;
  }
  atualizarContador();

  // Gera QR code da URL atual da página
  const qrcodeContainer = document.getElementById("qrcode");
  const urlAtual = window.location.href;
  QRCode.toCanvas(urlAtual, { width: 150 }, function (error, canvas) {
    if (error) console.error(error);
    else qrcodeContainer.appendChild(canvas);
  });
</script>
