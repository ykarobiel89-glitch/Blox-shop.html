# Blox-shop.html
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Blox Shop</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- Header -->
  <header>
    <img src="https://via.placeholder.com/80x80?text=Blox+Shop" alt="Logo Blox Shop" class="logo">
    <h1>Blox Shop</h1>
    <p>As melhores frutas do jogo em um só lugar!</p>
  </header>

  <!-- Filtros -->
  <div class="filtros">
    <button onclick="filtrar('todas')">Todas</button>
    <button onclick="filtrar('ate50')">Até R$ 50</button>
    <button onclick="filtrar('acima50')">Acima de R$ 50</button>
    <button onclick="filtrar('raras')">Frutas Raras</button>
    <input type="text" id="busca" placeholder="Buscar..." onkeyup="filtrarItens()">
  </div>

  <!-- Lista de itens -->
  <div id="lista-itens" class="grid"></div>

  <!-- Pop-up Pix -->
  <div id="popup-pix" class="popup">
    <div class="popup-content">
      <span class="fechar" onclick="fecharPix()">&times;</span>
      <h2 id="nome-item"></h2>
      <p>Para finalizar a compra no valor de <span id="preco-item"></span>, faça o pagamento via Pix:</p>
      <p class="pix-email">ykarobiel89@gmail.com</p>
      <img id="qr-code" src="" alt="QR Code Pix">
    </div>
  </div>

  <footer>
    © 2025 Blox Shop — Site fictício inspirado no jogo
  </footer>

  <script src="script.js"></script>
</body>
</html>
