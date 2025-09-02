<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Tabela de Gemas e Recursos</title>
  <style>
    body {
      background: #0b0f1a;
      font-family: Arial, sans-serif;
      color: #fff;
      display: flex;
      justify-content: center;
      padding: 40px;
    }


.recursos {
  position: relative;
  border: 3px solid transparent;
  border-radius: 12px;
  background: rgba(0, 255, 174, 0.05);
  padding: 20px;
  overflow: hidden;
  z-index: 1;
}

/* Borda futurista em gradiente neon */
.recursos::before {
  content: "";
  position: absolute;
  inset: 0;
  padding: 3px; /* espessura da borda */
  border-radius: 12px;
  background: linear-gradient(135deg, #00f0ff, #ff00ff, #00ffae);
  -webkit-mask: 
    linear-gradient(#fff 0 0) content-box, 
    linear-gradient(#fff 0 0);
  -webkit-mask-composite: xor;
          mask-composite: exclude;
  z-index: -1;
  filter: drop-shadow(0 0 12px #00f0ff) drop-shadow(0 0 20px #ff00ff) drop-shadow(0 0 25px #00ffae);
}

    .wrapper {
      display: flex;
      gap: 30px;
      align-items: flex-start;
    }

    /* Palavra vertical na esquerda */
    .lado-esquerdo {
      position: fixed;
      top: 50%;
      left: 0;
      transform: translateY(-50%) rotate(-90deg);
      font-size: 90px;
      font-weight: bold;
      letter-spacing: 5px;
      color: cyan;
      text-shadow: 2px 2px 6px rgba(0, 255, 255, 0.8), 
                   -2px -2px 6px rgba(0, 128, 128, 0.6);
      
    }


    .image-box img {
      max-width: 418px;
      border-radius: 12px;
      box-shadow: 0 0 25px #00c8ff;
    }

    .container {
      width: 800px;
    }

    h2 {
      margin: 10px 0;
      padding: 10px;
      text-transform: uppercase;
      font-size: 20px;
      font-weight: bold;
      color: #fff;
    }

    .section {
      margin-bottom: 30px;
      border-radius: 12px;
      padding: 20px;
    }

    .gemas {
      border: 2px solid #ff007f;
      background: rgba(255, 0, 127, 0.1);
      box-shadow: 0 0 20px #ff007f;
    }

    .recursos {
      border: 2px solid #00ffae;
      background: rgba(0, 255, 174, 0.1);
      box-shadow: 0 0 20px #00ffae;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 10px;
    }

    th, td {
      text-align: center;
      padding: 12px;
      font-size: 16px;
    }

    th {
      background: rgba(255, 255, 255, 0.1);
      font-weight: bold;
    }

    tr:nth-child(even) {
      background: rgba(255, 255, 255, 0.05);
    }
  </style>
</head>
<body>
  <div class="wrapper">
    <!-- IMAGEM -->

<div class="image-box" style="position: relative;">
  <img src="gato.jpeg" alt="Gato Guerreiro">
  <!-- Contato WhatsApp centralizado -->
  <a href="https://wa.me/5534997960026" target="_blank" 
     style="position: absolute; top: 95%; left: 40%; transform: translate(-30%, -50%);
            background: rgba(0,255,174,0.8); color: #fff; padding: 10px 20px;
            border-radius: 12px; font-weight: bold; font-size: 18px;
            text-decoration: none; display: flex; align-items: center; gap: 10px;
            box-shadow: 0 0 15px #00ffae;">
    <!-- Ícone do WhatsApp -->

    <span style="font-size: 24px;">📱</span> +55 34 99796-0026

  </a>
</div>


  <div class="lado-esquerdo">SMART FIT</div>

    <!-- CONTEÚDO -->
    <div class="container">
      <!-- GEMAS -->
      <div class="section gemas">
        <h2>💎 GEMAS</h2>
        <table>
          <tr>
            <th>Ícone</th>
            <th>Poder</th>
            <th>Preço</th>
          </tr>
          <tr>
            <td>💎</td>
            <td> 0 - 999M</td>
            <td>R$ 27,00</td>
          </tr>
          <tr>
            <td>💎💎</td>
            <td>1.000B - 1.399B</td>
            <td>R$ 28,00</td>
          </tr>
          <tr>
            <td>💎💎💎</td>
            <td>+1.399B</td>
            <td>R$ 29.50</td>
          </tr>
        </table>
      </div>

      <!-- RECURSOS -->
      <div class="section recursos">
        <h2>📦 RECURSOS</h2>
        <table>
          <tr>
            <th>Ícone</th>
            <th>Quantidades</th>
            <th>Preço</th>
          </tr>
          <tr>
            <td>🌾🪵🪨💎</td> 
            <td>1/1/1/1/0</td>
            <td>R$ 10,00</td>
          </tr>
          <tr>
            <td>🌾🪵🪨💎🪙</td>
            <td>1/1/1/1/1</td>
            <td>R$ 12,00</td>
          </tr>
          <tr>
            <td>🌾🪵🪨💎</td>
            <td>2/2/2/2/0</td>
            <td>R$ 16,00</td>
          </tr>
          <tr>
            <td>🌾🪵🪨💎🪙</td>
            <td>2/2/2/2/2</td>
            <td>R$ 20,00</td>
          </tr>
          <tr>
            <td>🌾🪵🪨💎</td>
            <td>4/4/4/4/2</td>
            <td>R$ 25,00</td>
          </tr>
          <tr>
            <td>🌾🪵🪨💎🪙</td>
            <td>4/4/4/4/4</td>
            <td>R$ 29,00</td>
          </tr>
        </table>
      </div>
    </div>
  </div>
</body>
</html>
