<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <title>Feliz Dia dos Namorados</title>
  <style>
    body {
      font-family: 'Georgia', serif;
      text-align: center;
      padding: 50px;
      background: linear-gradient(135deg, #ff9a9e 0%, #fad0c4 99%, #fad0c4 100%);
      color: #7a1f2f;
      min-height: 100vh;
      margin: 0;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }
    h1 {
      font-size: 3em;
      margin-bottom: 20px;
      font-weight: bold;
      text-shadow: 1px 1px 4px #fff0f0;
    }
    p {
      font-size: 1.5em;
      margin-bottom: 40px;
      font-style: italic;
    }
    img {
      max-width: 350px;
      border-radius: 25px;
      box-shadow: 0 8px 16px rgba(122, 31, 47, 0.6);
      margin: 0 auto;
    }
  </style>
</head>
<body>
  <h1>Feliz Dia dos Namorados!</h1>
  <p>Você é o meu melhor presente, hoje e sempre.</p>
  <img src="https://i.imgur.com/3xD2Z5g.jpg" alt="Romântico" />
</body>
</html>
Explicação rápida:
Fundo com um degradê rosa suave, super romântico.

Mensagem estilizada para o Dia dos Namorados.

Uma imagem de casal romântico (pode trocar a URL por outra se preferir).

Quando estiver pronto, você pode fazer o mesmo processo:

Criar um repositório novo, ou criar um arquivo index.html novo dentro do repositório que quiser.

Colar o código acima.

Salvar (commit).

Ativar o GitHub Pages (se for repositório novo).

Acessar o link.

Quer que eu te guie para criar o repositório e fazer tudo isso passo a passo de novo?







Você disse:
eu quero que você seja criativo, e crie um codigo para um site romantico, onde tenha coraçoes pulsantes, fundo rosa, espaço para colocar algumas fotos e um texto romantico 


O ChatGPT disse:
Claro, Igor! Vou criar um site romântico bem bacana pra você, com:

Fundo rosa suave;

Corações pulsando animados;

Espaço para até 3 fotos que você quiser (basta trocar as URLs);

Um texto romântico no centro;

Um visual delicado e moderno.

Segue o código completo que você pode usar direto no seu index.html:

html
Copiar
Editar
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <title>Amor que pulsa</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Parisienne&display=swap');

    body {
      margin: 0;
      background: #ffd1dc;
      font-family: 'Arial', sans-serif;
      color: #88002b;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 40px 20px;
      min-height: 100vh;
      overflow-x: hidden;
      position: relative;
    }

    h1 {
      font-family: 'Parisienne', cursive;
      font-size: 4em;
      margin-bottom: 0.2em;
      text-shadow: 2px 2px 5px #b3003b88;
    }

    p {
      max-width: 600px;
      font-size: 1.5em;
      text-align: center;
      margin-bottom: 40px;
      line-height: 1.4;
      font-weight: 500;
      text-shadow: 1px 1px 3px #c44160aa;
    }

    .photos {
      display: flex;
      gap: 20px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .photos img {
      width: 200px;
      height: 200px;
      object-fit: cover;
      border-radius: 20px;
      box-shadow: 0 4px 15px #b3003b66;
      transition: transform 0.3s ease;
      cursor: pointer;
    }
    .photos img:hover {
      transform: scale(1.1);
      box-shadow: 0 8px 30px #b3003bcc;
    }

    /* Corações pulsantes */
    .heart {
      position: fixed;
      width: 30px;
      height: 30px;
      background-color: #ff1e5f;
      left: 50%;
      top: 50%;
      transform-origin: center;
      animation: pulse 1.5s infinite ease-in-out;
      opacity: 0.7;
      clip-path: polygon(
        50% 0%, 
        61% 15%, 
        75% 15%, 
        84% 25%, 
        84% 40%, 
        75% 50%, 
        50% 75%, 
        25% 50%, 
        16% 40%, 
        16% 25%, 
        25% 15%, 
        39% 15%
      );
      filter: drop-shadow(0 0 3px #ff4f7d);
    }

    @keyframes pulse {
      0%, 100% {
        transform: translate(-50%, -50%) scale(1);
        opacity: 0.7;
      }
      50% {
        transform: translate(-50%, -50%) scale(1.3);
        opacity: 1;
      }
    }

    /* Vários corações em posições diferentes */
    .heart:nth-child(1) { top: 20%; left: 25%; animation-delay: 0s; }
    .heart:nth-child(2) { top: 30%; left: 75%; animation-delay: 0.5s; }
    .heart:nth-child(3) { top: 70%; left: 15%; animation-delay: 1s; }
    .heart:nth-child(4) { top: 80%; left: 70%; animation-delay: 1.2s; }
    .heart:nth-child(5) { top: 50%; left: 50%; animation-delay: 0.3s; }

  </style>
</head>
<body>
  <h1>Amor que pulsa</h1>
  <p>
    Nosso amor é feito de pequenos momentos, sorrisos trocados e corações que batem juntos, mesmo quando estamos longe.  
    Que cada dia seja uma nova página do nosso lindo livro de histórias.
  </p>

  <div class="photos">
    <img src="https://i.imgur.com/3xD2Z5g.jpg" alt="Foto romântica 1" />
    <img src="https://i.imgur.com/KlmZ9EC.jpg" alt="Foto romântica 2" />
    <img src="https://i.imgur.com/ebxRbDZ.jpg" alt="Foto romântica 3" />
  </div>

  <!-- Corações pulsantes -->
  <div class="heart"></div>
  <div class="heart"></div>
  <div class="heart"></div>
  <div class="heart"></div>
  <div class="heart"></div>

</body>
</html>
