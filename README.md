<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Alonso Díaz — Portfolio</title>
  <meta name="description" content="Portfolio de Alonso Díaz — Ingeniero de Computadores. Robótica, IA, Ciberseguridad y Computación de Altas Prestaciones." />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --muted:#98a0b3;
      --accent:#6ee7b7;
      --glass: rgba(255,255,255,0.04);
    }
    *{box-sizing:border-box}
    html,body{height:100%;}
    body{
      margin:0;
      font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,Helvetica,Arial;
      background:linear-gradient(180deg,#020617 0%, #07102a 60%);
      color:#e6eef8;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding:32px;
    }
    .container{max-width:1100px;margin:0 auto}
    header{
      display:flex;align-items:center;justify-content:space-between;margin-bottom:28px;
    }
    .brand{display:flex;align-items:center;gap:14px}
    .logo{width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,#5EEAD4,#60A5FA);display:flex;align-items:center;justify-content:center;font-weight:700;color:#032;box-shadow:0 6px 18px rgba(96,165,250,0.12)}
    h1{margin:0;font-size:clamp(20px,2.4vw,28px)}
    nav a{color:var(--muted);text-decoration:none;margin-left:18px}
    nav a:hover{color:var(--accent)}

    .hero{display:grid;grid-template-columns:1fr 360px;gap:28px;align-items:center;margin-bottom:28px}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent); padding:26px;border-radius:14px;box-shadow:0 8px 30px rgba(2,6,23,0.6);border:1px solid rgba(255,255,255,0.03)}
    .about h2{margin:0 0 8px 0}
    .roles{color:var(--muted);margin-bottom:14px}
    .cta{display:flex;gap:12px}
    .btn{background:var(--accent);color:#042; padding:10px 14px;border-radius:10px;font-weight:600;text-decoration:none}
    .btn.ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted)}

    .skills{display:flex;flex-wrap:wrap;gap:10px;margin-top:12px}
    .skill{background:var(--glass);padding:8px 12px;border-radius:999px;color:var(--muted);font-weight:600;font-size:13px}

    .stats{display:flex;gap:12px;margin-top:16px}
    .stat{background:linear-gradient(90deg, rgba(255,255,255,0.02), transparent);padding:12px;border-radius:10px;text-align:center;flex:1}
    .stat strong{display:block;font-size:18px}

    .projects{display:grid;grid-template-columns:repeat(auto-fill,minmax(240px,1fr));gap:16px;margin-top:20px}
    .project{padding:16px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.015), transparent);border:1px solid rgba(255,255,255,0.03)}
    .project h3{margin:0 0 8px 0}
    .project p{margin:0;color:var(--muted);font-size:14px}

    footer{display:flex;justify-content:space-between;align-items:center;margin-top:28px;color:var(--muted);font-size:14px}

    /* Responsive */
    @media (max-width:880px){
      .hero{grid-template-columns:1fr}
      nav{display:none}
    }

    /* Contact form */
    form{display:grid;gap:10px}
    input,textarea{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:10px;border-radius:8px;color:inherit}
    textarea{min-height:110px}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">AD</div>
        <div>
          <h1>Alonso Díaz</h1>
          <div style="color:var(--muted);font-size:13px">Ingeniero de Computadores — Robótica · IA · Ciberseguridad · Computación de Altas Prestaciones</div>
        </div>
      </div>
      <nav>
        <a href="#about">Sobre mí</a>
        <a href="#projects">Proyectos</a>
        <a href="#contact">Contacto</a>
      </nav>
    </header>

    <section class="hero">
      <div class="card about" id="about">
        <h2>Hola — soy Alonso</h2>
        <div class="roles">Ingeniero de Computadores</div>
        <p style="color:var(--muted);line-height:1.6">Me dedico a diseñar y desarrollar soluciones en robótica, inteligencia artificial, ciberseguridad y computación de altas prestaciones. Combino conocimiento en hardware y software para proyectos que requieren rendimiento, seguridad y autonomía.</p>
        <div class="skills">
          <span class="skill">Robótica</span>
          <span class="skill">Visión por Computador</span>
          <span class="skill">Aprendizaje Automático</span>
          <span class="skill">Ciberseguridad</span>
          <span class="skill">Sistemas Paralelos</span>
          <span class="skill">FPGA & SoC</span>
        </div>

        <div class="stats">
          <div class="stat"><strong>+5</strong><span style="color:var(--muted)">Años experiencia</span></div>
          <div class="stat"><strong>10+</strong><span style="color:var(--muted)">Proyectos</span></div>
          <div class="stat"><strong>3</strong><span style="color:var(--muted)">Publicaciones</span></div>
        </div>

        <div style="margin-top:16px" class="cta">
          <a class="btn" href="#contact">Contactar</a>
          <a class="btn ghost" href="#projects">Ver proyectos</a>
        </div>
      </div>

      <aside class="card">
        <h3>Contacto rápido</h3>
        <p style="color:var(--muted);margin-top:6px">¿Quieres colaborar? Escríbeme:</p>
        <ul style="padding-left:18px;color:var(--muted);margin-top:8px">
          <li>Email: <a href="mailto:alonso.diaz@example.com" style="color:var(--accent);text-decoration:none">alonso.diaz@example.com</a></li>
          <li>LinkedIn: <a href="#" style="color:var(--accent);text-decoration:none">/in/alonso-diaz</a></li>
          <li>GitHub: <a href="#" style="color:var(--accent);text-decoration:none">@alonso-diaz</a></li>
        </ul>
        <div style="margin-top:12px">
          <a class="btn" href="#">Descargar CV</a>
        </div>

        <hr style="margin:14px 0;border:none;border-top:1px solid rgba(255,255,255,0.03)" />
        <h4>Áreas</h4>
        <p style="color:var(--muted);margin:6px 0">Robótica · Inteligencia Artificial · Ciberseguridad · Computación de Altas Prestaciones</p>
      </aside>
    </section>

    <section id="projects">
      <h2 style="margin-bottom:12px">Proyectos seleccionados</h2>
      <div class="projects">
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
      </div>
    </section>

    <section id="contact" style="margin-top:26px">
      <h2>Contacto</h2>
      <div class="card" style="margin-top:10px">
        <form action="mailto:alonso.diaz@example.com" method="post" enctype="text/plain">
          <label>Nombre</label>
          <input type="text" name="name" placeholder="Tu nombre" />
          <label>Correo</label>
          <input type="email" name="email" placeholder="tu@ejemplo.com" />
          <label>Mensaje</label>
          <textarea name="message" placeholder="¿En qué proyecto quieres colaborar?"></textarea>
          <div style="display:flex;gap:10px;margin-top:6px">
            <button type="submit" class="btn">Enviar</button>
            <a class="btn ghost" href="#">Tel: +34 600 000 000</a>
          </div>
        </form>
      </div>
    </section>

    <footer>
      <div>© <span id="year"></span> Alonso Díaz — Ingeniero de Computadores</div>
      <div style="color:var(--muted)">Hecho con ♥ · Disponible para colaboraciones</div>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
