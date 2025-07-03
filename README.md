# Iantoken-
Token ianL
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>DistriCoin - Preventa Oficial</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet"/>
  <style>
    body {
      font-family: 'Montserrat', sans-serif;
      background-color: #0e0e0e;
      color: white;
      margin: 0;
      padding: 0;
    }
    header {
      background: linear-gradient(90deg, #0ff, #00f6ff);
      padding: 1.5rem;
      text-align: center;
      font-size: 1.6rem;
      font-weight: bold;
      color: black;
    }
    .container {
      padding: 2rem;
      max-width: 800px;
      margin: auto;
    }
    .token-info {
      background: #1a1a1a;
      padding: 1.5rem;
      border-radius: 1rem;
      margin-bottom: 2rem;
      box-shadow: 0 0 10px #00f6ff44;
    }
    .buy-section {
      background: #131313;
      padding: 2rem;
      border-radius: 1rem;
      text-align: center;
      box-shadow: 0 0 10px #0ff4;
    }
    input[type="number"] {
      padding: 0.5rem;
      width: 80%;
      border: none;
      border-radius: 0.5rem;
      font-size: 1rem;
      margin-bottom: 1rem;
    }
    button {
      background: #00f6ff;
      color: black;
      border: none;
      padding: 0.75rem 2rem;
      border-radius: 0.5rem;
      font-size: 1.1rem;
      font-weight: bold;
      cursor: pointer;
    }
    footer {
      text-align: center;
      margin-top: 3rem;
      font-size: 0.9rem;
      color: gray;
    }
  </style>
</head>
<body>

  <header>
    🚀 Preventa Oficial de DistriCoin (DSTC)
  </header>

  <div class="container">
    <div class="token-info">
      <h2>📊 Detalles del Token</h2>
      <p><strong>Nombre:</strong> DistriCoin</p>
      <p><strong>Símbolo:</strong> DSTC</p>
      <p><strong>Red:</strong> BNB Smart Chain (BEP20)</p>
      <p><strong>Precio preventa:</strong> 1 DSTC = 0.01 USDT</p>
      <p><strong>Soft Cap:</strong> 5,000 USDT</p>
      <p><strong>Hard Cap:</strong> 20,000 USDT</p>
    </div>

    <div class="buy-section">
      <h2>💰 Participa en la Preventa</h2>
      <p>Conecta tu wallet y compra tus tokens antes del lanzamiento</p>
      <input type="number" id="usdtInput" placeholder="Ingrese cantidad en USDT">
      <br>
      <button onclick="buyTokens()">Comprar DSTC</button>
    </div>

    <footer>
      🔒 100% seguro | Liquidez bloqueada al finalizar la preventa <br />
      📧 Soporte: contacto@districoin.io
    </footer>
  </div>

  <script>
    function buyTokens() {
      const amount = document.getElementById('usdtInput').value;
      if (!amount || amount <= 0) {
        alert('Ingrese una cantidad válida');
        return;
      }
      alert('Se enviará la solicitud para comprar ' + (amount / 0.01) + ' DSTC');
      // Aquí iría la conexión a Web3 (MetaMask) + contrato de preventa
    }
  </script>
</body>
</html>
