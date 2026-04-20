<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>O Poder Invisível da Mente</title>
  <style>
    :root {
      --bg: #050505;
      --bg-soft: #0d0d0d;
      --card: #111111;
      --card-2: #161616;
      --text: #ffffff;
      --muted: #b8b8b8;
      --accent: #ff2a2a;
      --accent-2: #00d4ff;
      --border: rgba(255,255,255,0.08);
      --shadow: 0 10px 30px rgba(0,0,0,.35);
    }

    body.light {
      --bg: #f5f5f5;
      --bg-soft: #ffffff;
      --card: #ffffff;
      --card-2: #f2f2f2;
      --text: #111111;
      --muted: #555555;
      --accent: #d90000;
      --accent-2: #0087a8;
      --border: rgba(0,0,0,0.08);
      --shadow: 0 10px 30px rgba(0,0,0,.08);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: radial-gradient(circle at top, #151515 0%, var(--bg) 45%);
      color: var(--text);
      line-height: 1.5;
      transition: background .3s ease, color .3s ease;
    }

    .topbar {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      z-index: 999;
      background: rgba(0,0,0,.82);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid var(--border);
    }

    body.light .topbar {
      background: rgba(255,255,255,.88);
    }

    .topbar-inner {
      max-width: 1180px;
      margin: 0 auto;
      padding: 14px 18px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
    }

    .timer-box {
      font-weight: 700;
      font-size: 15px;
      color: var(--text);
    }

    .timer-box span {
      color: var(--accent);
    }

    .theme-toggle {
      border: 1px solid var(--border);
      background: var(--card);
      color: var(--text);
      border-radius: 999px;
      padding: 10px 14px;
      cursor: pointer;
      font-weight: 700;
    }

    .container {
      max-width: 1180px;
      margin: 0 auto;
      padding: 92px 20px 60px;
    }

    .hero {
      min-height: 92vh;
      display: grid;
      grid-template-columns: 1.1fr .9fr;
      align-items: center;
      gap: 34px;
    }

    .hero-text h1 {
      font-size: clamp(2.2rem, 5vw, 4.6rem);
      line-height: .95;
      text-transform: uppercase;
      margin-bottom: 18px;
      font-weight: 900;
    }

    .hero-text h1 span {
      color: var(--accent);
    }

    .hero-text p {
      font-size: clamp(1rem, 2vw, 1.25rem);
      color: var(--muted);
      max-width: 620px;
      margin-bottom: 26px;
    }

    .cta-row {
      display: flex;
      gap: 14px;
      flex-wrap: wrap;
      margin-bottom: 24px;
    }

    .btn {
      display: inline-block;
      padding: 16px 24px;
      border-radius: 14px;
      text-decoration: none;
      font-weight: 800;
      transition: .25s ease;
      text-align: center;
      border: 1px solid transparent;
    }

    .btn-primary {
      background: linear-gradient(90deg, var(--accent), #ff5252);
      color: #fff;
      box-shadow: 0 10px 24px rgba(255, 42, 42, .22);
    }

    .btn-primary:hover {
      transform: translateY(-2px);
      filter: brightness(1.05);
    }

    .btn-secondary {
      background: transparent;
      border-color: var(--border);
      color: var(--text);
    }

    .hero-card {
      background: linear-gradient(180deg, var(--card), var(--card-2));
      border: 1px solid var(--border);
      border-radius: 24px;
      padding: 24px;
      box-shadow: var(--shadow);
      position: relative;
      overflow: hidden;
    }

    .hero-card::before {
      content: "";
      position: absolute;
      inset: -30%;
      background: radial-gradient(circle, rgba(255,42,42,.18) 0%, transparent 60%);
      pointer-events: none;
    }

    .book-mockup {
      position: relative;
      background: #0a0a0a;
      border: 1px solid rgba(255,255,255,.08);
      border-radius: 22px;
      padding: 28px 22px;
      min-height: 470px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      overflow: hidden;
    }

    body.light .book-mockup {
      background: #f7f7f7;
    }

    .brain {
      width: 180px;
      height: 180px;
      border-radius: 50%;
      position: relative;
      margin-bottom: 24px;
      background:
        radial-gradient(circle at 35% 35%, rgba(255,255,255,.06), transparent 20%),
        radial-gradient(circle at 65% 65%, rgba(255,255,255,.04), transparent 18%),
        #111;
      border: 3px solid #222;
      box-shadow: inset 0 0 30px rgba(255,255,255,.03), 0 0 25px rgba(255,42,42,.12);
    }

    .brain::before, .brain::after {
      content: "";
      position: absolute;
      top: 12px;
      width: 44%;
      height: 156px;
      border: 3px solid #2e2e2e;
      border-radius: 80px;
      background:
        repeating-linear-gradient(
          90deg,
          rgba(255,255,255,.02) 0 7px,
          rgba(0,0,0,.0) 7px 14px
        ),
        #0f0f0f;
    }

    .brain::before { left: 8px; }
    .brain::after { right: 8px; }

    .arrow {
      position: absolute;
      width: 78px;
      height: 4px;
      background: #0f0f0f;
      border-radius: 99px;
      transform-origin: left center;
      box-shadow: 0 0 8px rgba(255,255,255,.03);
    }

    .arrow::after {
      content: "";
      position: absolute;
      right: -2px;
      top: -6px;
      border-left: 14px solid #0f0f0f;
      border-top: 8px solid transparent;
      border-bottom: 8px solid transparent;
    }

    .a1 { top: 88px; left: 18px; transform: rotate(18deg); }
    .a2 { top: 42px; left: 75px; transform: rotate(55deg); width: 64px; }
    .a3 { top: 32px; right: 78px; transform: rotate(125deg); width: 64px; }
    .a4 { top: 88px; right: 18px; transform: rotate(162deg); }
    .a5 { bottom: 70px; left: 38px; transform: rotate(-25deg); width: 70px; }
    .a6 { bottom: 70px; right: 38px; transform: rotate(205deg); width: 70px; }

    .book-title {
      font-size: clamp(2rem, 4vw, 3.3rem);
      line-height: .95;
      font-weight: 900;
      text-transform: uppercase;
      margin-bottom: 10px;
    }

    .book-title .accent {
      color: var(--accent);
    }

    .book-sub {
      color: var(--muted);
      font-size: 1rem;
      max-width: 420px;
    }

    .stats {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 16px;
      margin-top: 22px;
    }

    .stat {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 18px;
      text-align: center;
      box-shadow: var(--shadow);
    }

    .stat .num {
      font-size: 1.9rem;
      font-weight: 900;
      color: var(--accent-2);
    }

    .section {
      padding: 76px 0;
    }

    .section-title {
      font-size: clamp(1.8rem, 4vw, 3rem);
      text-transform: uppercase;
      margin-bottom: 18px;
      font-weight: 900;
    }

    .section-title span {
      color: var(--accent);
    }

    .section-text {
      max-width: 860px;
      color: var(--muted);
      font-size: 1.08rem;
    }

    .grid-2 {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 22px;
      margin-top: 30px;
    }

    .card {
      background: linear-gradient(180deg, var(--card), var(--card-2));
      border: 1px solid var(--border);
      border-radius: 22px;
      padding: 26px;
      box-shadow: var(--shadow);
    }

    .card h3 {
      font-size: 1.35rem;
      margin-bottom: 10px;
      text-transform: uppercase;
    }

    .card p {
      color: var(--muted);
    }

    .benefits {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 18px;
      margin-top: 30px;
    }

    .benefit {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 20px;
      padding: 22px;
    }

    .benefit strong {
      display: block;
      margin-bottom: 8px;
      color: var(--text);
      font-size: 1.08rem;
    }

    .benefit p {
      color: var(--muted);
      font-size: .98rem;
    }

    .final-cta {
      text-align: center;
      background: linear-gradient(180deg, rgba(255,42,42,.08), transparent);
      border: 1px solid var(--border);
      border-radius: 26px;
      padding: 38px 24px;
      margin-top: 24px;
    }

    .final-cta h2 {
      font-size: clamp(2rem, 4vw, 3.3rem);
      text-transform: uppercase;
      margin-bottom: 14px;
    }

    .final-cta p {
      color: var(--muted);
      max-width: 760px;
      margin: 0 auto 22px;
    }

    .floating-whatsapp {
      position: fixed;
      bottom: 20px;
      right: 20px;
      z-index: 999;
      width: 58px;
      height: 58px;
      display: grid;
      place-items: center;
      border-radius: 50%;
      background: #25d366;
      color: white;
      text-decoration: none;
      font-size: 1.5rem;
      font-weight: 900;
      box-shadow: 0 10px 25px rgba(37,211,102,.35);
    }

    .sales-popup {
      position: fixed;
      left: 18px;
      bottom: 18px;
      z-index: 999;
      min-width: 260px;
      max-width: 320px;
      background: var(--card);
      color: var(--text);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 14px 16px;
      box-shadow: var(--shadow);
      opacity: 0;
      transform: translateY(20px);
      transition: .35s ease;
      pointer-events: none;
    }

    .sales-popup.show {
      opacity: 1;
      transform: translateY(0);
    }

    .sales-popup strong {
      color: var(--accent-2);
      display: block;
      margin-bottom: 4px;
    }

    .exit-popup {
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,.82);
      z-index: 1000;
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
    }

    .exit-popup.active {
      display: flex;
    }

    .exit-box {
      width: 100%;
      max-width: 560px;
      background: var(--bg-soft);
      border: 1px solid var(--border);
      border-radius: 24px;
      padding: 30px 24px;
      text-align: center;
      box-shadow: var(--shadow);
    }

    .exit-box h3 {
      font-size: clamp(1.8rem, 4vw, 2.6rem);
      margin-bottom: 12px;
      text-transform: uppercase;
    }

    .exit-box p {
      color: var(--muted);
      margin-bottom: 22px;
    }

    .reveal {
      opacity: 0;
      transform: translateY(36px);
      transition: opacity .7s ease, transform .7s ease;
    }

    .reveal.visible {
      opacity: 1;
      transform: translateY(0);
    }

    @media (max-width: 980px) {
      .hero,
      .grid-2,
      .benefits,
      .stats {
        grid-template-columns: 1fr;
      }

      .hero {
        min-height: auto;
        padding-top: 10px;
      }

      .hero-card {
        order: -1;
      }

      .topbar-inner {
        padding: 12px 14px;
      }

      .timer-box {
        font-size: 13px;
      }
    }
  </style>
</head>
<body>
  <div class="topbar">
    <div class="topbar-inner">
      <div class="timer-box">⏰ Oferta expira em <span id="countdown">10:00</span></div>
      <button class="theme-toggle" id="themeToggle">Modo Dark/Light</button>
    </div>
  </div>

  <main class="container">
    <section class="hero">
      <div class="hero-text reveal">
        <h1>Domine sua mente <span>ou continue sendo dominado</span></h1>
        <p>
          Você não está sem capacidade. Você só está sendo travado pela própria mente.
          “O Poder Invisível da Mente” foi criado para quebrar procrastinação, autossabotagem
          e falta de disciplina.
        </p>

        <div class="cta-row">
          <a href="https://SEU_LINK_DA_KIWIFY" class="btn btn-primary">QUERO ACESSO IMEDIATO</a>
          <a href="https://wa.me/55SEUNUMERO" class="btn btn-secondary">TIRAR DÚVIDAS NO WHATSAPP</a>
        </div>

        <div class="stats">
          <div class="stat">
            <div class="num" data-target="250">0</div>
            <div>Leitores impactados</div>
          </div>
          <div class="stat">
            <div class="num" data-target="10">0</div>
            <div>Minutos de urgência</div>
          </div>
          <div class="stat">
            <div class="num" data-target="100">0</div>
            <div>Foco na ação</div>
          </div>
        </div>
      </div>

      <div class="hero-card reveal">
        <div class="book-mockup">
          <div class="arrow a1"></div>
          <div class="arrow a2"></div>
          <div class="arrow a3"></div>
          <div class="arrow a4"></div>
          <div class="arrow a5"></div>
          <div class="arrow a6"></div>
          <div class="brain"></div>
          <div class="book-title">O Poder Invisível <span class="accent">da Mente</span></div>
          <div class="book-sub">
            Pare de se sabotar. Assuma o controle. Saia do ciclo da procrastinação e entre em ação.
          </div>
        </div>
      </div>
    </section>

    <section class="section reveal">
      <h2 class="section-title">A <span>dor principal</span></h2>
      <p class="section-text">
        O verdadeiro problema não é falta de inteligência, nem falta de oportunidade.
        É saber exatamente o que precisa ser feito e ainda assim não fazer. É viver travado,
        adiar decisões, começar e parar, prometer mudança e continuar no mesmo lugar.
        A dor principal é a sensação de estar sendo derrotado pela própria mente.
      </p>
    </section>

    <section class="section">
      <div class="grid-2">
        <div class="card reveal">
          <h3>O problema</h3>
          <p>
            Sua mente te condiciona ao conforto, à distração e ao adiamento. Isso gera culpa,
            frustração e a sensação de que seu potencial está sendo desperdiçado.
          </p>
        </div>
        <div class="card reveal">
          <h3>O objetivo</h3>
          <p>
            Fazer você recuperar controle mental, criar disciplina real e agir mesmo sem motivação.
            O foco não é te animar por um dia. É te transformar em alguém que executa.
          </p>
        </div>
      </div>
    </section>

    <section class="section reveal">
      <h2 class="section-title">O que esse eBook <span>resolve</span></h2>
      <p class="section-text">
        “O Poder Invisível da Mente” resolve procrastinação, autossabotagem, falta de consistência
        e ausência de direção. Ele mostra por que você trava, como sua mente te manipula
        e como quebrar esse padrão com ação prática.
      </p>

      <div class="benefits">
        <div class="benefit reveal">
          <strong>Mais disciplina</strong>
          <p>Você passa a agir sem depender de vontade ou motivação passageira.</p>
        </div>
        <div class="benefit reveal">
          <strong>Menos procrastinação</strong>
          <p>Você reduz adiamento e começa a cumprir o que promete para si mesmo.</p>
        </div>
        <div class="benefit reveal">
          <strong>Mais controle</strong>
          <p>Você assume comando sobre pensamentos, foco e decisões.</p>
        </div>
        <div class="benefit reveal">
          <strong>Mais clareza</strong>
          <p>Você entende por que trava e identifica o padrão que estava te sabotando.</p>
        </div>
        <div class="benefit reveal">
          <strong>Mais ação</strong>
          <p>Seu comportamento deixa de ser paralisado e começa a avançar de verdade.</p>
        </div>
        <div class="benefit reveal">
          <strong>Transformação real</strong>
          <p>Não é motivação vazia. É mentalidade aplicada à execução.</p>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="final-cta reveal">
        <h2>Ou você assume o controle <span style="color: var(--accent);">agora</span>…</h2>
        <p>
          …ou continua sendo controlado pela procrastinação, pela dúvida e pela autossabotagem.
          A decisão que muda sua vida não acontece amanhã. Ela acontece quando você age.
        </p>
        <div class="cta-row" style="justify-content:center;">
          <a href="https://SEU_LINK_DA_KIWIFY" class="btn btn-primary">QUERO COMEÇAR AGORA</a>
          <a href="https://wa.me/55SEUNUMERO" class="btn btn-secondary">FALAR NO WHATSAPP</a>
        </div>
      </div>
    </section>
  </main>

  <a class="floating-whatsapp" href="https://wa.me/55SEUNUMERO" aria-label="WhatsApp">W</a>

  <div class="sales-popup" id="salesPopup">
    <strong>Compra recente</strong>
    <div id="salesPopupText">Lucas acabou de adquirir o eBook.</div>
  </div>

  <div class="exit-popup" id="exitPopup">
    <div class="exit-box">
      <h3>Espera… você vai sair agora?</h3>
      <p>
        Se você fechar essa página, nada muda. Você continua no mesmo ciclo.
        Aproveite enquanto a oferta ainda está disponível.
      </p>
      <div class="cta-row" style="justify-content:center;">
        <a href="https://SEU_LINK_DA_KIWIFY" class="btn btn-primary">ÚLTIMA CHANCE DE ACESSO</a>
        <button class="btn btn-secondary" id="closeExitPopup">Continuar na página</button>
      </div>
    </div>
  </div>

  <script>
    // Tema dark/light
    const themeToggle = document.getElementById("themeToggle");
    themeToggle.addEventListener("click", () => {
      document.body.classList.toggle("light");
    });

    // Countdown 10 minutos
    const countdownEl = document.getElementById("countdown");
    let totalSeconds = 10 * 60;

    function updateCountdown() {
      const minutes = Math.floor(totalSeconds / 60).toString().padStart(2, "0");
      const seconds = (totalSeconds % 60).toString().padStart(2, "0");
      countdownEl.textContent = `${minutes}:${seconds}`;

      if (totalSeconds > 0) {
        totalSeconds--;
      }
    }
    updateCountdown();
    setInterval(updateCountdown, 1000);

    // Scroll reveal
    const reveals = document.querySelectorAll(".reveal");
    const revealObserver = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add("visible");
        }
      });
    }, { threshold: 0.15 });

    reveals.forEach(el => revealObserver.observe(el));

    // Contador numérico
    const counters = document.querySelectorAll(".num");
    const counterObserver = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (!entry.isIntersecting) return;
        const el = entry.target;
        const target = +el.getAttribute("data-target");
        let current = 0;
        const step = Math.max(1, Math.ceil(target / 40));

        const interval = setInterval(() => {
          current += step;
          if (current >= target) {
            current = target;
            clearInterval(interval);
          }
          el.textContent = current;
        }, 35);

        counterObserver.unobserve(el);
      });
    }, { threshold: 0.5 });

    counters.forEach(counter => counterObserver.observe(counter));

    // Popup de vendas
    const salesPopup = document.getElementById("salesPopup");
    const salesPopupText = document.getElementById("salesPopupText");

    const salesMessages = [
      "Lucas acabou de adquirir o eBook.",
      "Daniel comprou há 2 minutos.",
      "Ana liberou o acesso agora.",
      "Juliana garantiu o conteúdo.",
      "Mais uma pessoa entrou agora."
    ];

    let salesIndex = 0;

    function showSalesPopup() {
      salesPopupText.textContent = salesMessages[salesIndex];
      salesPopup.classList.add("show");

      setTimeout(() => {
        salesPopup.classList.remove("show");
      }, 3500);

      salesIndex = (salesIndex + 1) % salesMessages.length;
    }

    setTimeout(showSalesPopup, 2500);
    setInterval(showSalesPopup, 7000);

    // Popup de saída
    const exitPopup = document.getElementById("exitPopup");
    const closeExitPopup = document.getElementById("closeExitPopup");
    let exitShown = false;

    document.addEventListener("mouseout", function(e) {
      if (!exitShown && e.clientY <= 0) {
        exitPopup.classList.add("active");
        exitShown = true;
      }
    });

    closeExitPopup.addEventListener("click", () => {
      exitPopup.classList.remove("active");
    });
  </script>
</body>
</html>
