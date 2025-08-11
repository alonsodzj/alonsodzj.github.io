<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Alonso Díaz — Portfolio</title>
  <meta name="description" content="Portfolio de Alonso Díaz — Ingeniero de Computadores. Robótica, IA, Ciberseguridad y Computación de Altas Prestaciones." />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #fafafa;
      --text: #111111;
      --muted: #666666;
      --accent: #000000;
      --divider: #e0e0e0;
      --btn-bg: transparent;
      --btn-hover-bg: #000000;
      --btn-hover-color: #fafafa;
    }

    * {
      box-sizing: border-box;
    }
    html, body {
      margin: 0;
      padding: 0;
      font-family: "Inter", system-ui, -apple-system, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      background-color: var(--bg);
      color: var(--text);
      height: 100%;
    }

    .container {
      max-width: 900px;
      margin: 0 auto;
      padding: 40px 20px;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding-bottom: 40px;
      border-bottom: 1px solid var(--divider);
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 16px;
    }

    .logo {
      font-weight: 700;
      font-size: 32px;
      color: var(--accent);
      user-select: none;
    }

    h1 {
      margin: 0;
      font-weight: 700;
      font-size: 28px;
    }

    nav a {
      text-decoration: none;
      color: var(--muted);
      font-weight: 600;
      margin-left: 24px;
      transition: color 0.3s ease;
      font-size: 14px;
    }

    nav a:hover {
      color: var(--accent);
    }

    .hero {
      margin: 60px 0;
      max-width: 600px;
    }

    .hero h2 {
      font-weight: 700;
      font-size: 48px;
      margin-bottom: 16px;
      line-height: 1.1;
    }

    .roles {
      font-weight: 500;
      font-size: 18px;
      color: var(--muted);
      margin-bottom: 24px;
    }

    .hero p {
      font-size: 18px;
      line-height: 1.6;
      color: var(--muted);
      margin-bottom: 32px;
    }

    .skills {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      margin-bottom: 48px;
    }

    .skill {
      font-weight: 600;
      font-size: 14px;
      color: var(--accent);
      border-bottom: 2px solid var(--accent);
      padding-bottom: 2px;
    }

    .cta {
      display: flex;
      gap: 16px;
    }

    .btn {
      cursor: pointer;
      font-weight: 700;
      font-size: 14px;
      padding: 14px 24px;
      border: none;
      background-color: var(--btn-bg);
      color: var(--accent);
      transition: background-color 0.3s ease, color 0.3s ease;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      border-radius: 6px;
    }

    .btn:hover {
      background-color: var(--btn-hover-bg);
      color: var(--btn-hover-color);
    }

    #projects {
      margin-bottom: 60px;
    }

    #projects h2 {
      font-weight: 700;
      font-size: 32px;
      margin-bottom: 24px;
      color: var(--text);
    }

    .project {
      margin-bottom: 40px;
    }

    .project h3 {
      font-weight: 700;
      font-size: 20px;
      margin-bottom: 8px;
      color: var(--text);
    }

    .project p {
      font-size: 16px;
      color: var(--muted);
      line-height: 1.5;
      margin: 0;
    }

    #contact {
      margin-bottom: 60px;
    }

    #contact h2 {
      font-weight: 700;
      font-size: 32px;
      margin-bottom: 24px;
      color: var(--text);
    }

    form {
      display: grid;
      gap: 16px;
      max-width: 600px;
    }

    label {
      font-weight: 600;
      font-size: 14px;
      color: var(--text);
    }

    input, textarea {
      background: transparent;
      border: 1px solid var(--divider);
      padding: 12px;
      border-radius: 6px;
      font-size: 16px;
      color: var(--text);
      font-family: inherit;
      resize: vertical;
      transition: border-color 0.3s ease;
    }

    input:focus, textarea:focus {
      outline: none;
      border-color: var(--accent);
    }

    textarea {
      min-height: 120px;
    }

    footer {
      border-top: 1px solid var(--divider);
      padding: 24px 0;
      font-size: 14px;
      color: var(--muted);
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 12px;
    }

    /* Responsive */

    @media (max-width: 768px) {
      header {
        flex-direction: column;
        align-items: flex-start;
      }
      nav {
        margin-top: 20px;
      }
      nav a {
        margin-left: 0;
        margin-right: 24px;
        font-size: 16px;
      }
      .hero h2 {
        font-size: 36px;
      }
      .btn {
        padding: 12px 20px;
        font-size: 16px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">AD</div>
        <div>
          <h1>Alonso Díaz</h1>
          <div style="color:var(--muted);font-size:13px; margin-top:4px;">
            Ingeniero de Computadores — Robótica · IA · Ciberseguridad · Computación de Altas Prestaciones
          </div>
        </div>
      </div>
      <nav>
        <a href="#about">Sobre mí</a>
        <a href="#projects">Proyectos</a>
        <a href="#contact">Contacto</a>
      </nav>
    </header>

    <section class="hero" id="about">
      <h2>Hola — soy Alonso</h2>
      <div class="roles">Ingeniero de Computadores</div>
      <p>Me dedico a diseñar y desarrollar soluciones en robótica, inteligencia artificial, ciberseguridad y computación de altas prestaciones. Combino conocimiento en hardware y software para proyectos que requieren rendimiento, seguridad y autonomía.</p>

      <div class="skills">
        <span class="skill">Robótica</span>
        <span class="skill">Visión por Computador</span>
        <span class="skill">Aprendizaje Automático</span>
        <span class="skill">Ciberseguridad</span>
        <span class="skill">Sistemas Paralelos</span>
        <span class="skill">FPGA & SoC</span>
      </div>

      <div class="cta">
        <a class="btn" href="#contact">Contactar</a>
        <a class="btn" href="#projects">Ver proyectos</a>
      </div>
    </section>

    <section id="projects">
      <h2>Proyectos seleccionados</h2>
      <article class="project">
        <h3>Plataforma robótica autónoma</h3>
        <p>Desarrollo de un robot móvil con navegación SLAM y planificación en tiempo real. Integración de sensores LIDAR y cámaras, con control en FPGA para la capa de tiempo real.</p>
      </article>

      <article class="project">
        <h3>Sistema de detección de intrusiones basado en IA</h3>
        <p>Detector de ataques en red usando modelos de aprendizaje profundo optimizados para inferencia en edge devices.</p>
      </article>

      <article class="project">
        <h3>Cluster de cómputo para HPC</h3>
        <p>Diseño e implementación de un clúster con balanceo de carga, aceleradores y optimizaciones para cargas científicas paralelas.</p>
      </article>

      <article class="project">
        <h3>Pipeline de visión industrial</h3>
        <p>Cadena completa desde adquisición hasta clasificación en tiempo real, con optimizaciones SIMD y uso de CUDA cuando aplica.</p>
      </article>
    </section>

    <section id="contact">
      <h2>Contacto</h2>
      <form action="mailto:alonso.diaz@example.com" method="post" enctype="text/plain" novalidate>
        <label for="name">Nombre</label>
        <input type="text" id="name" name="name" placeholder="Tu nombre" required />

        <label for="email">Correo</label>
        <input type="email" id="email" name="email" placeholder="tu@ejemplo.com" required />

        <label for="message">Mensaje</label>
        <textarea id="message" name="message" placeholder="¿En qué proyecto quieres colaborar?" required></textarea>

        <div style="display:flex;gap:10px; margin-top: 6px;">
          <button type="submit" class="btn">Enviar</button>
          <a class="btn" href="tel:+34600000000">Tel: +34 600 000 000</a>
        </div>
      </form>
    </section>

    <footer>
      <div>© <span id="year"></span> Alonso Díaz — Ingeniero de Computadores</div>
      <div>Hecho con ♥ · Disponible para colaboraciones</div>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
