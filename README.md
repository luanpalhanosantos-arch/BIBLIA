
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="theme-color" content="#080808" />

  <title>JESUS IS KING | Palavra de Deus</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700;900&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    :root {
      --gold: #d9b66f;
      --white: #f5f0e6;
      --black: #080808;
    }

    body {
      background: var(--black);
      color: var(--white);
      font-family: 'Inter', sans-serif;
      min-height: 100vh;
    }

    /* Cabeçalho */
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 25px 8%;
      border-bottom: 1px solid #ffffff15;
      position: relative;
      z-index: 2;
    }

    .logo {
      font-family: 'Cinzel', serif;
      color: var(--gold);
      font-size: 19px;
      font-weight: 700;
      letter-spacing: 3px;
    }

    header span {
      font-size: 11px;
      letter-spacing: 3px;
      color: #c9c2b5;
    }

    /* Seção principal */
    .hero {
      min-height: 690px;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 70px 8%;
      position: relative;
      overflow: hidden;

      background:
        linear-gradient(
          90deg,
          rgba(8,8,8,0.98) 0%,
          rgba(8,8,8,0.88) 45%,
          rgba(8,8,8,0.40) 100%
        ),
        url("https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=2000&q=85")
        center / cover no-repeat;
    }

    .hero-content {
      width: 100%;
      max-width: 1100px;
      position: relative;
      z-index: 1;
    }

    .eyebrow {
      color: var(--gold);
      font-size: 12px;
      letter-spacing: 5px;
      margin-bottom: 25px;
      text-transform: uppercase;
    }

    h1 {
      font-family: 'Cinzel', serif;
      font-size: clamp(45px, 8vw, 92px);
      line-height: 1.12;
      font-weight: 700;
      max-width: 800px;
    }

    h1 span {
      display: block;
      color: var(--gold);
    }

    .subtitle {
      color: #c7c2b8;
      font-size: 16px;
      line-height: 1.9;
      max-width: 490px;
      margin-top: 24px;
    }

    .gold-line {
      width: 75px;
      height: 2px;
      background: var(--gold);
      margin: 30px 0;
    }

    .button {
      border: 1px solid var(--gold);
      color: var(--gold);
      background: transparent;
      padding: 15px 25px;
      display: inline-block;
      text-decoration: none;
      font-size: 11px;
      letter-spacing: 2px;
      text-transform: uppercase;
      cursor: pointer;
      transition: 0.3s;
    }

    .button:hover {
      color: #080808;
      background: var(--gold);
    }

    /* Versículo */
    .verse-section {
      padding: 100px 8%;
      text-align: center;
      background:
        radial-gradient(ellipse at center, #302719 0%, #11100d 42%, #080808 75%);
    }

    .section-label {
      color: var(--gold);
      font-size: 11px;
      letter-spacing: 5px;
      text-transform: uppercase;
    }

    .verse-section h2 {
      font-family: 'Cinzel', serif;
      font-size: clamp(25px, 4vw, 42px);
      margin: 25px auto;
      font-weight: 400;
    }

    .verse-text {
      max-width: 760px;
      margin: 0 auto;
      font-size: clamp(19px, 3vw, 27px);
      line-height: 1.8;
      font-weight: 300;
      color: #eee6d8;
    }

    .verse-reference {
      color: var(--gold);
      margin-top: 28px;
      letter-spacing: 2px;
      font-size: 13px;
    }

    .verse-button {
      margin-top: 35px;
    }

    /* Jesus is King */
    .king-section {
      min-height: 550px;
      padding: 90px 8%;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      position: relative;
      overflow: hidden;

      background:
        linear-gradient(#0009, #000b),
        url("https://images.unsplash.com/photo-1519681393784-d120267933ba?auto=format&fit=crop&w=2000&q=85")
        center / cover no-repeat;
    }

    .king-content {
      position: relative;
      z-index: 1;
    }

    .cross {
      color: var(--gold);
      font-size: 48px;
      margin-bottom: 22px;
    }

    .king-title {
      font-family: 'Cinzel', serif;
      font-weight: 900;
      font-size: clamp(43px, 9vw, 105px);
      line-height: 1.15;
      letter-spacing: 5px;
      text-shadow: 0 5px 35px #000;
    }

    .king-title span {
      color: var(--gold);
      display: block;
    }

    .king-subtitle {
      margin-top: 25px;
      font-size: 12px;
      letter-spacing: 5px;
      color: #e0d6c2;
    }

    /* Rodapé */
    footer {
      padding: 35px 20px;
      text-align: center;
      border-top: 1px solid #ffffff12;
      color: #888176;
      font-size: 12px;
      line-height: 2;
    }

    footer strong {
      color: var(--gold);
      font-family: 'Cinzel', serif;
      letter-spacing: 2px;
    }

    @media (max-width: 600px) {
      header {
        padding: 22px 6%;
      }

      .logo {
        font-size: 15px;
        letter-spacing: 2px;
      }

      header span {
        font-size: 9px;
        letter-spacing: 1px;
      }

      .hero {
        min-height: 600px;
        padding: 60px 7%;
        background-position: 60% center;
      }

      .verse-section {
        padding: 75px 7%;
      }

      .king-section {
        min-height: 440px;
        padding: 70px 5%;
      }

      .king-title {
        letter-spacing: 2px;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="logo">✝ JESUS IS KING</div>
    <span>FÉ • ESPERANÇA • AMOR</span>
  </header>

  <main>
    <section class="hero">
      <div class="hero-content">
        <p class="eyebrow">A palavra que transforma</p>

        <h1>
          A fé move
          <span>montanhas.</span>
        </h1>

        <div class="gold-line"></div>

        <p class="subtitle">
          Em meio ao caos do mundo, existe uma verdade
          que nunca muda: Jesus Cristo é o caminho,
          a verdade e a vida.
        </p>

        <a href="#versiculo" class="button">
          Receber a palavra ↓
        </a>
      </div>
    </section>

    <section class="verse-section" id="versiculo">
      <p class="section-label">✦ Palavra de Deus ✦</p>

      <h2>Versículo para sua vida</h2>

      <p class="verse-text" id="verseText" aria-live="polite">
        Carregando uma palavra de esperança...
      </p>

      <p class="verse-reference" id="verseReference"></p>

      <button class="button verse-button" id="newVerse">
        Novo versículo ↗
      </button>
    </section>

    <section class="king-section">
      <div class="king-content">
        <div class="cross">✝</div>

        <h2 class="king-title">
          JESUS
          <span>IS KING</span>
        </h2>

        <p class="king-subtitle">
          REI DOS REIS • SENHOR DOS SENHORES
        </p>
      </div>
    </section>
  </main>

  <footer>
    <strong>JESUS IS KING</strong>
    <p>“A Ele seja a glória para todo o sempre.”</p>
    <p>Vivendo pela fé. Caminhando com Cristo. ❤️</p>
  </footer>

  <script>
    const verses = [
      {
        text: "O Senhor é o meu pastor; nada me faltará.",
        reference: "Salmos 23:1"
      },
      {
        text: "Tudo posso naquele que me fortalece.",
        reference: "Filipenses 4:13"
      },
      {
        text: "Porque vivemos por fé, e não pelo que vemos.",
        reference: "2 Coríntios 5:7"
      },
      {
        text: "Eu sou o caminho, e a verdade e a vida.",
        reference: "João 14:6"
      },
      {
        text: "Não temas, porque eu sou contigo.",
        reference: "Isaías 41:10"
      },
      {
        text: "Entrega o teu caminho ao Senhor; confia nele.",
        reference: "Salmos 37:5"
      },
      {
        text: "O amor é paciente, o amor é bondoso.",
        reference: "1 Coríntios 13:4"
      },
      {
        text: "Buscai primeiro o Reino de Deus e a sua justiça.",
        reference: "Mateus 6:33"
      },
      {
        text: "Deixo-vos a paz, a minha paz vos dou.",
        reference: "João 14:27"
      },
      {
        text: "A minha graça te basta, porque o meu poder se aperfeiçoa na fraqueza.",
        reference: "2 Coríntios 12:9"
      },
      {
        text: "Confia no Senhor de todo o teu coração.",
        reference: "Provérbios 3:5"
      },
      {
        text: "Sede fortes e corajosos; não temais.",
        reference: "Deuteronômio 31:6"
      },
      {
        text: "Nós amamos porque ele nos amou primeiro.",
        reference: "1 João 4:19"
      },
      {
        text: "Perto está o Senhor dos que têm o coração quebrantado.",
        reference: "Salmos 34:18"
      },
      {
        text: "Se Deus é por nós, quem será contra nós?",
        reference: "Romanos 8:31"
      }
    ];

    const verseText = document.getElementById("verseText");
    const verseReference = document.getElementById("verseReference");
    const newVerseButton = document.getElementById("newVerse");

    let previousIndex = -1;

    function showRandomVerse() {
      let index;

      do {
        index = Math.floor(Math.random() * verses.length);
      } while (verses.length > 1 && index === previousIndex);

      previousIndex = index;

      verseText.textContent = "“" + verses[index].text + "”";
      verseReference.textContent = "— " + verses[index].reference;
    }

    // Um versículo aleatório ao abrir a página.
    showRandomVerse();

    // Permite ao visitante sortear outro versículo.
    newVerseButton.addEventListener("click", showRandomVerse);
  </script>

</body>
</html>
