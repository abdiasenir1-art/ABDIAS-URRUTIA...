<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ABDIAS URRUTIA</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto+Slab:wght@400;700;900&family=Nunito:wght@400;600;700;800&family=Orbitron:wght@700;900&display=swap" rel="stylesheet"/>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-behavior: smooth; font-size: 16px; }
    body {
      background: linear-gradient(180deg, #060a14 0%, #0a0e1a 30%, #0d1220 100%);
      color: #f0f4ff;
      font-family: 'Nunito', sans-serif;
      min-height: 100vh;
    }

    ::-webkit-scrollbar { width: 6px; }
    ::-webkit-scrollbar-track { background: #0a0e1a; }
    ::-webkit-scrollbar-thumb { background: #6366f1; border-radius: 3px; }

    @keyframes float {
      from { transform: translateY(0px) scale(1); }
      to   { transform: translateY(-30px) scale(1.1); }
    }
    @keyframes shimmer {
      0%   { background-position: -200% center; }
      100% { background-position:  200% center; }
    }
    @keyframes pulse-ring {
      0%   { transform: scale(0.9); opacity: 1; }
      100% { transform: scale(1.6); opacity: 0; }
    }
    @keyframes fadeSlideUp {
      from { opacity: 0; transform: translateY(30px); }
      to   { opacity: 1; transform: translateY(0); }
    }
    @keyframes cardIn {
      from { opacity: 0; transform: translateY(60px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    /* ---- PARTICLES ---- */
    .particles { position: fixed; inset: 0; pointer-events: none; overflow: hidden; z-index: 0; }
    .particle {
      position: absolute;
      border-radius: 50%;
      opacity: 0.13;
      animation: float 4s ease-in-out infinite alternate;
    }
    .grid-bg {
      position: absolute; inset: 0;
      background-image:
        linear-gradient(rgba(99,102,241,0.03) 1px, transparent 1px),
        linear-gradient(90deg, rgba(99,102,241,0.03) 1px, transparent 1px);
      background-size: 60px 60px;
    }

    /* ---- NAV ---- */
    nav {
      position: sticky; top: 0; z-index: 50;
      display: flex; align-items: center; justify-content: space-between;
      padding: 1rem 1.5rem;
      background: rgba(6,10,20,0.88);
      backdrop-filter: blur(20px);
      border-bottom: 1px solid rgba(255,255,255,0.06);
    }
    .nav-logo {
      font-family: 'Orbitron', sans-serif;
      font-weight: 900; font-size: 1.1rem;
      letter-spacing: 0.2em; text-transform: uppercase;
      background: linear-gradient(135deg, #a5b4fc, #818cf8);
      -webkit-background-clip: text; -webkit-text-fill-color: transparent;
      text-decoration: none;
    }
    .nav-links { display: flex; gap: 0.5rem; flex-wrap: wrap; justify-content: flex-end; }
    .nav-link {
      font-size: 0.75rem; font-weight: 700;
      padding: 0.35rem 0.85rem; border-radius: 9999px;
      text-decoration: none; transition: all 0.2s;
      border: 1px solid transparent;
      color: #64748b;
    }
    .nav-link:hover { color: #c7d2fe; background: rgba(99,102,241,0.1); border-color: rgba(99,102,241,0.4); }

    /* ---- HERO ---- */
    header {
      position: relative; z-index: 10;
      text-align: center; padding: 5rem 1.5rem 6rem;
      overflow: hidden;
    }
    .ring {
      position: absolute; inset: 0;
      display: flex; align-items: center; justify-content: center;
      pointer-events: none;
    }
    .ring-circle {
      width: 500px; height: 500px; border-radius: 50%;
      border: 1px solid rgba(99,102,241,0.07);
      animation: pulse-ring 5s ease-out infinite;
    }
    .hero-label {
      font-size: 0.8rem; font-weight: 700;
      text-transform: uppercase; letter-spacing: 0.4em;
      color: #6366f1; margin-bottom: 1rem;
      animation: fadeSlideUp 0.7s ease both;
    }
    .hero-title {
      font-family: 'Roboto Slab', serif;
      font-size: clamp(3.5rem, 10vw, 7rem);
      font-weight: 900; text-transform: uppercase;
      line-height: 1; letter-spacing: -0.02em;
      margin-bottom: 1.5rem;
      background: linear-gradient(135deg, #ffffff 0%, #c7d2fe 40%, #818cf8 70%, #6366f1 100%);
      background-size: 200% auto;
      -webkit-background-clip: text; -webkit-text-fill-color: transparent;
      animation: shimmer 4s linear infinite, fadeSlideUp 0.8s ease both;
    }
    .hero-sub {
      font-size: 1.05rem; color: #94a3b8;
      max-width: 520px; margin: 0 auto 2.5rem;
      animation: fadeSlideUp 0.9s ease both 0.1s;
    }
    .hero-buttons { display: flex; flex-wrap: wrap; gap: 1rem; justify-content: center; }
    .hero-btn {
      display: flex; align-items: center; gap: 0.5rem;
      padding: 0.75rem 1.4rem; border-radius: 1rem;
      font-weight: 700; font-size: 0.9rem;
      color: #fff; text-decoration: none;
      transition: transform 0.25s, box-shadow 0.25s;
      font-family: 'Nunito', sans-serif;
    }
    .hero-btn:hover { transform: scale(1.06); }
    .hero-btn .icon { font-size: 1.15rem; }

    /* ---- DIVIDER ---- */
    .rainbow-divider {
      position: relative; z-index: 10;
      max-width: 900px; margin: 0 auto 4rem; padding: 0 1.5rem;
    }
    .rainbow-divider::after {
      content: ''; display: block; height: 1px; width: 100%;
      background: linear-gradient(90deg,
        transparent,
        rgba(99,102,241,0.5),
        rgba(16,185,129,0.5),
        rgba(249,115,22,0.5),
        rgba(34,197,94,0.5),
        transparent);
    }

    /* ---- CARDS ---- */
    main { position: relative; z-index: 10; max-width: 1100px; margin: 0 auto; padding: 0 1.5rem 6rem; }

    .subject-card {
      position: relative; overflow: hidden; border-radius: 1.75rem;
      margin-bottom: 4rem;
      border: 1px solid;
      background: linear-gradient(135deg, #0f172a 0%, #111827 100%);
      opacity: 0; transform: translateY(60px);
      transition: opacity 0.7s ease, transform 0.7s ease;
    }
    .subject-card.visible { opacity: 1; transform: translateY(0); }

    .card-top-bar { height: 6px; width: 100%; }

    .card-inner {
      display: flex; flex-direction: column;
    }
    @media (min-width: 900px) {
      .card-inner { flex-direction: row; }
      .card-inner.reverse { flex-direction: row-reverse; }
    }

    .card-image-wrap {
      position: relative; overflow: hidden;
      flex-shrink: 0;
    }
    @media (min-width: 900px) {
      .card-image-wrap { width: 40%; min-height: 420px; }
    }
    .card-image-wrap img {
      width: 100%; height: 300px; object-fit: cover;
      transition: transform 0.7s ease;
      display: block;
    }
    @media (min-width: 900px) {
      .card-image-wrap img { height: 100%; min-height: 420px; }
    }
    .card-image-wrap:hover img { transform: scale(1.05); }
    .card-img-overlay { position: absolute; inset: 0; }
    .card-emoji {
      position: absolute; bottom: 1.5rem; left: 1.5rem;
      width: 3.5rem; height: 3.5rem; border-radius: 1rem;
      display: flex; align-items: center; justify-content: center;
      font-size: 1.75rem;
    }

    .card-content {
      flex: 1; padding: 2.5rem 3rem;
      display: flex; flex-direction: column; justify-content: center;
    }
    @media (max-width: 899px) { .card-content { padding: 2rem 1.75rem; } }

    .card-title {
      font-family: 'Roboto Slab', serif;
      font-size: clamp(2rem, 4vw, 3rem);
      font-weight: 900; margin-bottom: 0.5rem;
      line-height: 1.1;
    }
    .card-tags { display: flex; flex-wrap: wrap; gap: 0.5rem; margin-bottom: 1.5rem; margin-top: 0.75rem; }
    .tag {
      font-size: 0.7rem; font-weight: 700;
      padding: 0.3rem 0.85rem; border-radius: 9999px;
      text-transform: uppercase; letter-spacing: 0.15em;
      border: 1px solid;
    }
    .card-desc p { line-height: 1.75; margin-bottom: 0.9rem; }
    .card-desc p:last-child { margin-bottom: 0; }
    .card-desc p.lead { color: #e2e8f0; font-weight: 600; font-size: 1rem; }
    .card-desc p.body { color: #94a3b8; font-size: 0.95rem; }

    /* ---- FOOTER ---- */
    footer {
      position: relative; z-index: 10;
      text-align: center; padding: 3rem 1.5rem;
      border-top: 1px solid rgba(255,255,255,0.06);
    }
    .footer-name {
      font-family: 'Orbitron', sans-serif;
      font-size: 1.5rem; font-weight: 900;
      text-transform: uppercase; letter-spacing: 0.2em;
      background: linear-gradient(135deg, #818cf8, #6366f1);
      -webkit-background-clip: text; -webkit-text-fill-color: transparent;
      margin-bottom: 0.5rem;
    }
    .footer-sub { font-size: 0.85rem; color: #475569; }
  </style>
</head>
<body>

<!-- Particles -->
<div class="particles">
  <div class="grid-bg"></div>
  <div class="particle" style="left:5%;top:10%;width:80px;height:80px;background:#6366f1;animation-delay:0s;animation-duration:4s;"></div>
  <div class="particle" style="left:85%;top:20%;width:60px;height:60px;background:#10b981;animation-delay:1.2s;animation-duration:5s;"></div>
  <div class="particle" style="left:70%;top:65%;width:100px;height:100px;background:#f97316;animation-delay:0.6s;animation-duration:3.5s;"></div>
  <div class="particle" style="left:15%;top:75%;width:70px;height:70px;background:#22c55e;animation-delay:1.8s;animation-duration:4.5s;"></div>
  <div class="particle" style="left:50%;top:5%;width:50px;height:50px;background:#6366f1;animation-delay:2.4s;animation-duration:3s;"></div>
  <div class="particle" style="left:95%;top:50%;width:40px;height:40px;background:#f59e0b;animation-delay:0.9s;animation-duration:5.5s;"></div>
</div>

<!-- Nav -->
<nav>
  <a href="#top" class="nav-logo">A·U</a>
  <div class="nav-links">
    <a href="#matematicas"      class="nav-link">📐 Matemáticas</a>
    <a href="#informatica"      class="nav-link">💻 Informática</a>
    <a href="#educacion-fisica" class="nav-link">⚽ Ed. Física</a>
    <a href="#ciencias"         class="nav-link">🌿 Cs. Naturales</a>
  </div>
</nav>

<!-- Hero -->
<header id="top">
  <div class="ring"><div class="ring-circle"></div></div>
  <p class="hero-label">Examen Final · 2026</p>
  <h1 class="hero-title">ABDIAS<br>URRUTIA</h1>
  <p class="hero-sub">Temario completo de materias para el examen. Explora cada sección con su descripción detallada.</p>
  <div class="hero-buttons">
    <a href="#matematicas"      class="hero-btn" style="background:linear-gradient(135deg,#4338ca,#6366f1);box-shadow:0 4px 20px rgba(99,102,241,0.35);"><span class="icon">📐</span> Matemáticas</a>
    <a href="#informatica"      class="hero-btn" style="background:linear-gradient(135deg,#059669,#10b981);box-shadow:0 4px 20px rgba(16,185,129,0.35);"><span class="icon">💻</span> Informática</a>
    <a href="#educacion-fisica" class="hero-btn" style="background:linear-gradient(135deg,#ea580c,#f97316);box-shadow:0 4px 20px rgba(249,115,22,0.35);"><span class="icon">⚽</span> Ed. Física</a>
    <a href="#ciencias"         class="hero-btn" style="background:linear-gradient(135deg,#16a34a,#22c55e);box-shadow:0 4px 20px rgba(34,197,94,0.35);"><span class="icon">🌿</span> Cs. Naturales</a>
  </div>
</header>

<div class="rainbow-divider"></div>

<main>

  <!-- MATEMÁTICAS -->
  <article id="matematicas" class="subject-card" style="border-color:rgba(99,102,241,0.45);box-shadow:0 0 60px rgba(99,102,241,0.12),0 25px 50px rgba(0,0,0,0.5);">
    <div class="card-top-bar" style="background:linear-gradient(90deg,#4338ca,#6366f1,#818cf8);"></div>
    <div class="card-inner">
      <div class="card-image-wrap">
        <img src="https://images.unsplash.com/photo-1635070041078-e363dbe005cb?w=800&h=500&fit=crop&auto=format" alt="Ecuaciones matemáticas en una pizarra"/>
        <div class="card-img-overlay" style="background:linear-gradient(to right,transparent 40%,#111827 100%),linear-gradient(to top,rgba(67,56,202,0.6) 0%,transparent 60%);"></div>
        <div class="card-emoji" style="background:#6366f1;box-shadow:0 0 30px rgba(99,102,241,0.4);">📐</div>
      </div>
      <div class="card-content">
        <h2 class="card-title" style="background:linear-gradient(135deg,#818cf8,#6366f1);-webkit-background-clip:text;-webkit-text-fill-color:transparent;">Matemáticas</h2>
        <div class="card-tags">
          <span class="tag" style="background:rgba(99,102,241,0.12);color:#818cf8;border-color:rgba(99,102,241,0.4);">Álgebra</span>
          <span class="tag" style="background:rgba(99,102,241,0.12);color:#818cf8;border-color:rgba(99,102,241,0.4);">Geometría</span>
          <span class="tag" style="background:rgba(99,102,241,0.12);color:#818cf8;border-color:rgba(99,102,241,0.4);">Trigonometría</span>
          <span class="tag" style="background:rgba(99,102,241,0.12);color:#818cf8;border-color:rgba(99,102,241,0.4);">Estadística</span>
          <span class="tag" style="background:rgba(99,102,241,0.12);color:#818cf8;border-color:rgba(99,102,241,0.4);">Cálculo</span>
          <span class="tag" style="background:rgba(99,102,241,0.12);color:#818cf8;border-color:rgba(99,102,241,0.4);">Probabilidad</span>
        </div>
        <div class="card-desc">
          <p class="lead">Las Matemáticas son la ciencia que estudia las propiedades de los números, las figuras geométricas, las estructuras abstractas y las relaciones entre ellas mediante el uso del razonamiento lógico y deductivo. Es considerada el lenguaje universal de la ciencia, ya que permite describir con precisión los fenómenos del mundo natural y social.</p>
          <p class="body">En el nivel secundario, las Matemáticas abarcan un amplio espectro de temas fundamentales como el álgebra, que estudia las operaciones con variables y expresiones simbólicas; la geometría, que analiza las formas, ángulos, áreas y volúmenes en el espacio; la aritmética, que trabaja con las operaciones básicas y propiedades de los números enteros, racionales e irracionales; y las funciones matemáticas, que describen relaciones entre conjuntos de valores.</p>
          <p class="body">El estudio de la trigonometría nos permite comprender las relaciones entre los ángulos y los lados de los triángulos, herramienta clave en la arquitectura, la ingeniería y la navegación. La estadística y la probabilidad nos enseñan a recolectar, organizar e interpretar datos, habilidades esenciales en el mundo moderno donde la toma de decisiones basada en evidencia es prioritaria.</p>
          <p class="body">Las Matemáticas desarrollan habilidades cognitivas de alto nivel como el pensamiento crítico, la resolución sistemática de problemas, el razonamiento abstracto y la capacidad de argumentar con lógica. Estas destrezas trascienden las aulas y son aplicables en todas las áreas del conocimiento humano, desde la física y la química hasta la economía, la música y las artes.</p>
        </div>
      </div>
    </div>
  </article>

  <!-- INFORMÁTICA -->
  <article id="informatica" class="subject-card" style="border-color:rgba(16,185,129,0.45);box-shadow:0 0 60px rgba(16,185,129,0.12),0 25px 50px rgba(0,0,0,0.5);">
    <div class="card-top-bar" style="background:linear-gradient(90deg,#059669,#10b981,#34d399);"></div>
    <div class="card-inner reverse">
      <div class="card-image-wrap">
        <img src="https://images.unsplash.com/photo-1517694712202-14dd9538aa97?w=800&h=500&fit=crop&auto=format" alt="Pantalla de computadora con código"/>
        <div class="card-img-overlay" style="background:linear-gradient(to left,transparent 40%,#111827 100%),linear-gradient(to top,rgba(5,150,105,0.6) 0%,transparent 60%);"></div>
        <div class="card-emoji" style="background:#10b981;box-shadow:0 0 30px rgba(16,185,129,0.4);">💻</div>
      </div>
      <div class="card-content">
        <h2 class="card-title" style="background:linear-gradient(135deg,#34d399,#10b981);-webkit-background-clip:text;-webkit-text-fill-color:transparent;">Informática</h2>
        <div class="card-tags">
          <span class="tag" style="background:rgba(16,185,129,0.12);color:#34d399;border-color:rgba(16,185,129,0.4);">Hardware</span>
          <span class="tag" style="background:rgba(16,185,129,0.12);color:#34d399;border-color:rgba(16,185,129,0.4);">Software</span>
          <span class="tag" style="background:rgba(16,185,129,0.12);color:#34d399;border-color:rgba(16,185,129,0.4);">Programación</span>
          <span class="tag" style="background:rgba(16,185,129,0.12);color:#34d399;border-color:rgba(16,185,129,0.4);">Redes</span>
          <span class="tag" style="background:rgba(16,185,129,0.12);color:#34d399;border-color:rgba(16,185,129,0.4);">Bases de Datos</span>
          <span class="tag" style="background:rgba(16,185,129,0.12);color:#34d399;border-color:rgba(16,185,129,0.4);">Inteligencia Artificial</span>
        </div>
        <div class="card-desc">
          <p class="lead">La Informática es la ciencia que se ocupa del tratamiento automático de la información mediante el uso de computadoras y sistemas digitales. Integra conocimientos de matemáticas, ingeniería eléctrica, lógica y comunicación para diseñar sistemas capaces de procesar, almacenar y transmitir datos de manera eficiente y confiable.</p>
          <p class="body">El estudio de la Informática comienza con la comprensión de los componentes físicos del computador, llamados hardware: el procesador (CPU), la memoria RAM, el disco duro, la tarjeta gráfica, la placa madre y los dispositivos de entrada y salida. Cada componente cumple una función específica dentro del sistema y trabaja de forma coordinada para ejecutar las instrucciones del usuario.</p>
          <p class="body">El software es la contraparte lógica del hardware. Los sistemas operativos como Windows, Linux o macOS son programas que administran los recursos del computador y permiten ejecutar otras aplicaciones. Los lenguajes de programación como Python, Java, JavaScript, C++ y muchos más permiten a los desarrolladores escribir instrucciones que las máquinas pueden interpretar y ejecutar.</p>
          <p class="body">En la era digital actual, la Informática es transversal a todas las profesiones. La inteligencia artificial, el aprendizaje automático, la ciberseguridad, el desarrollo web y las aplicaciones móviles son áreas de frontera que transforman continuamente nuestra forma de vivir, trabajar y comunicarnos. Aprender Informática hoy es prepararse para el futuro del trabajo y la innovación global.</p>
        </div>
      </div>
    </div>
  </article>

  <!-- EDUCACIÓN FÍSICA -->
  <article id="educacion-fisica" class="subject-card" style="border-color:rgba(249,115,22,0.45);box-shadow:0 0 60px rgba(249,115,22,0.12),0 25px 50px rgba(0,0,0,0.5);">
    <div class="card-top-bar" style="background:linear-gradient(90deg,#ea580c,#f97316,#fb923c);"></div>
    <div class="card-inner">
      <div class="card-image-wrap">
        <img src="https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?w=800&h=500&fit=crop&auto=format" alt="Estudiantes practicando deportes"/>
        <div class="card-img-overlay" style="background:linear-gradient(to right,transparent 40%,#111827 100%),linear-gradient(to top,rgba(234,88,12,0.6) 0%,transparent 60%);"></div>
        <div class="card-emoji" style="background:#f97316;box-shadow:0 0 30px rgba(249,115,22,0.4);">⚽</div>
      </div>
      <div class="card-content">
        <h2 class="card-title" style="background:linear-gradient(135deg,#fb923c,#f97316);-webkit-background-clip:text;-webkit-text-fill-color:transparent;">Educación Física</h2>
        <div class="card-tags">
          <span class="tag" style="background:rgba(249,115,22,0.12);color:#fb923c;border-color:rgba(249,115,22,0.4);">Atletismo</span>
          <span class="tag" style="background:rgba(249,115,22,0.12);color:#fb923c;border-color:rgba(249,115,22,0.4);">Deportes Colectivos</span>
          <span class="tag" style="background:rgba(249,115,22,0.12);color:#fb923c;border-color:rgba(249,115,22,0.4);">Gimnasia</span>
          <span class="tag" style="background:rgba(249,115,22,0.12);color:#fb923c;border-color:rgba(249,115,22,0.4);">Salud y Nutrición</span>
          <span class="tag" style="background:rgba(249,115,22,0.12);color:#fb923c;border-color:rgba(249,115,22,0.4);">Natación</span>
          <span class="tag" style="background:rgba(249,115,22,0.12);color:#fb923c;border-color:rgba(249,115,22,0.4);">Primeros Auxilios</span>
        </div>
        <div class="card-desc">
          <p class="lead">La Educación Física es una disciplina educativa que promueve el desarrollo integral del ser humano a través del movimiento, el ejercicio físico, el deporte y el juego. Más allá de la actividad corporal, busca formar personas saludables, disciplinadas, cooperativas y con valores éticos que les permitan desenvolverse exitosamente en la sociedad.</p>
          <p class="body">El cuerpo humano es una máquina extraordinaria que requiere cuidado y ejercicio constante para mantenerse en óptimas condiciones. A través de la Educación Física se trabajan las capacidades físicas condicionales: la resistencia cardiovascular y muscular, la fuerza, la velocidad y la flexibilidad. Estas capacidades se complementan con las habilidades coordinativas como el equilibrio, la orientación espacial, el ritmo y la reacción.</p>
          <p class="body">Los deportes colectivos como el fútbol, el baloncesto, el voleibol y el béisbol enseñan valores fundamentales como el trabajo en equipo, el respeto por las reglas, la comunicación efectiva, la solidaridad y el manejo de la victoria y la derrota con dignidad. Los deportes individuales como el atletismo, la natación y la gimnasia fortalecen la autodisciplina, la perseverancia y la confianza en uno mismo.</p>
          <p class="body">La actividad física regular tiene comprobados beneficios para la salud física y mental. Reduce el riesgo de enfermedades cardiovasculares, diabetes y obesidad; mejora la postura, la coordinación y la agilidad; libera endorfinas que reducen el estrés y la ansiedad; y favorece un sueño reparador. La Educación Física forma el hábito de vida activa que acompañará a los estudiantes durante toda su vida adulta.</p>
        </div>
      </div>
    </div>
  </article>

  <!-- CIENCIAS NATURALES -->
  <article id="ciencias" class="subject-card" style="border-color:rgba(34,197,94,0.45);box-shadow:0 0 60px rgba(34,197,94,0.12),0 25px 50px rgba(0,0,0,0.5);">
    <div class="card-top-bar" style="background:linear-gradient(90deg,#16a34a,#22c55e,#4ade80);"></div>
    <div class="card-inner reverse">
      <div class="card-image-wrap">
        <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=800&h=500&fit=crop&auto=format" alt="Laboratorio de ciencias con microscopio"/>
        <div class="card-img-overlay" style="background:linear-gradient(to left,transparent 40%,#111827 100%),linear-gradient(to top,rgba(22,163,74,0.6) 0%,transparent 60%);"></div>
        <div class="card-emoji" style="background:#22c55e;box-shadow:0 0 30px rgba(34,197,94,0.4);">🌿</div>
      </div>
      <div class="card-content">
        <h2 class="card-title" style="background:linear-gradient(135deg,#4ade80,#22c55e);-webkit-background-clip:text;-webkit-text-fill-color:transparent;">Ciencias Naturales</h2>
        <div class="card-tags">
          <span class="tag" style="background:rgba(34,197,94,0.12);color:#4ade80;border-color:rgba(34,197,94,0.4);">Biología Celular</span>
          <span class="tag" style="background:rgba(34,197,94,0.12);color:#4ade80;border-color:rgba(34,197,94,0.4);">Química Orgánica</span>
          <span class="tag" style="background:rgba(34,197,94,0.12);color:#4ade80;border-color:rgba(34,197,94,0.4);">Física Clásica</span>
          <span class="tag" style="background:rgba(34,197,94,0.12);color:#4ade80;border-color:rgba(34,197,94,0.4);">Ecología</span>
          <span class="tag" style="background:rgba(34,197,94,0.12);color:#4ade80;border-color:rgba(34,197,94,0.4);">Genética</span>
          <span class="tag" style="background:rgba(34,197,94,0.12);color:#4ade80;border-color:rgba(34,197,94,0.4);">Astronomía</span>
        </div>
        <div class="card-desc">
          <p class="lead">Las Ciencias Naturales constituyen un conjunto de disciplinas científicas dedicadas al estudio de la naturaleza y sus fenómenos desde una perspectiva empírica y experimental. Comprenden la Biología, la Física, la Química, la Geología y la Astronomía, y utilizan el método científico como herramienta principal para generar conocimiento validado y reproducible.</p>
          <p class="body">La Biología estudia los seres vivos en toda su diversidad y complejidad, desde las moléculas que forman las células hasta los ecosistemas completos. Abarca la genética y la herencia de características, la evolución de las especies, la fisiología de los organismos, la ecología de las poblaciones y la taxonomía que clasifica a los millones de especies que habitan la Tierra. La célula es la unidad básica de la vida, y su estudio revela los secretos del funcionamiento de todo ser vivo.</p>
          <p class="body">La Química es la ciencia de la materia y sus transformaciones. Estudia la composición, estructura y propiedades de las sustancias, así como los cambios que experimentan durante las reacciones químicas. La tabla periódica de los elementos organiza los 118 elementos conocidos según sus propiedades, y es una de las herramientas más poderosas de la ciencia moderna. Los conceptos de ácidos, bases, soluciones, enlaces químicos y reacciones orgánicas son pilares de esta disciplina.</p>
          <p class="body">La Física describe las leyes fundamentales que gobiernan el universo: el movimiento, la gravedad, la electricidad, el magnetismo, el calor, el sonido y la luz. Las leyes de Newton explican por qué los planetas orbitan el sol y por qué caen los objetos. La física cuántica revela el comportamiento extraño de las partículas subatómicas. Las Ciencias Naturales en su conjunto nos invitan a observar el mundo con curiosidad y a formular preguntas que expanden los límites del conocimiento humano.</p>
        </div>
      </div>
    </div>
  </article>

</main>

<!-- Footer -->
<footer>
  <p class="footer-name">ABDIAS URRUTIA</p>
  <p class="footer-sub">Examen Final 2026 · Matemáticas · Informática · Educación Física · Ciencias Naturales</p>
</footer>

<script>
  // Scroll reveal animation
  const cards = document.querySelectorAll('.subject-card');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach((entry, i) => {
      if (entry.isIntersecting) {
        setTimeout(() => entry.target.classList.add('visible'), i * 80);
        observer.unobserve(entry.target);
      }
    });
  }, { threshold: 0.1 });
  cards.forEach(card => observer.observe(card));

  // Nav active state
  const navLinks = document.querySelectorAll('.nav-link');
  window.addEventListener('scroll', () => {
    const ids = ['matematicas','informatica','educacion-fisica','ciencias'];
    let active = '';
    for (const id of ids.slice().reverse()) {
      const el = document.getElementById(id);
      if (el && el.getBoundingClientRect().top <= 200) { active = id; break; }
    }
    navLinks.forEach(link => {
      const href = link.getAttribute('href').replace('#','');
      if (href === active) {
        link.style.color = '#c7d2fe';
        link.style.background = 'rgba(99,102,241,0.12)';
        link.style.borderColor = 'rgba(99,102,241,0.4)';
      } else {
        link.style.color = '#64748b';
        link.style.background = 'transparent';
        link.style.borderColor = 'transparent';
      }
    });
  });
</script>
</body>
</html>
