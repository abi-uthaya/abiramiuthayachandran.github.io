# abiramiuthayachandran.github.io
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>[Your Name] — Portfolio</title>
  <meta name="description" content="Portfolio of [Your Name] — Projects, skills, and contact." />
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#94a3b8; --accent:#7c3aed; --glass: rgba(255,255,255,0.03);
      --max-w:1100px; --radius:14px; --gap:18px; --pad:20px;
      font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
      color-scheme: dark;
    }

    *{box-sizing:border-box}
    html,body{height:100%; margin:0; background:linear-gradient(180deg,var(--bg),#071024); color:#e6eef8}
    a{color:inherit}

    .wrap{max-width:var(--max-w); margin:40px auto; padding:24px}

    header{display:flex; align-items:center; justify-content:space-between; gap:12px}
    .brand{display:flex; align-items:center; gap:14px}
    .logo{width:52px;height:52px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#2dd4bf);display:flex;align-items:center;justify-content:center;font-weight:700}
    nav a{margin-left:14px; color:var(--muted); text-decoration:none; font-weight:600}

    .hero{display:grid; grid-template-columns:1fr 360px; gap:28px; margin-top:28px}
    .card{background:var(--card); border-radius:var(--radius); padding:var(--pad); box-shadow:0 6px 30px rgba(2,6,23,0.6)}

    .intro h1{margin:0 0 8px 0; font-size:28px}
    .intro p{margin:0 0 12px 0; color:var(--muted)}
    .cta{display:flex; gap:12px}
    .btn{background:var(--accent); padding:10px 14px; border-radius:10px; font-weight:700; color:white; text-decoration:none}
    .ghost{background:transparent; border:1px solid rgba(255,255,255,0.06); color:var(--muted); padding:10px 14px; border-radius:10px}

    .profile{display:flex; flex-direction:column; gap:12px; align-items:center}
    .avatar{width:100%; max-width:240px; aspect-ratio:1/1; border-radius:12px; background:linear-gradient(180deg,#082032,#0b2540); display:flex;align-items:center;justify-content:center; font-size:20px; color:var(--muted)}
    .meta{width:100%; text-align:center}
    .meta h3{margin:6px 0}
    .meta p{margin:0; color:var(--muted)}

    /* Projects grid */
    .projects{margin-top:28px}
    .grid{display:grid; grid-template-columns:repeat(auto-fit,minmax(230px,1fr)); gap:var(--gap)}
    .proj{padding:14px; border-radius:12px; background:linear-gradient(180deg, rgba(255,255,255,0.02), var(--glass)); border:1px solid rgba(255,255,255,0.03)}
    .proj h4{margin:8px 0}
    .proj p{margin:0 0 10px 0; color:var(--muted); font-size:14px}
    .tags{display:flex; gap:8px; flex-wrap:wrap}
    .tag{font-size:12px; padding:6px 8px; border-radius:8px; background:rgba(255,255,255,0.02); color:var(--muted)}

    .skills{display:flex; gap:12px; flex-wrap:wrap; margin-top:12px}
    .skill{padding:8px 12px; border-radius:999px; background:rgba(255,255,255,0.02); color:var(--muted); font-weight:600}

    footer{margin-top:40px; text-align:center; color:var(--muted); font-size:14px}

    @media (max-width:900px){
      .hero{grid-template-columns:1fr}
      nav{display:none}
      .wrap{margin:20px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">AB</div>
        <div>
          <div style="font-weight:800">[Your Name]</div>
          <div style="font-size:13px;color:var(--muted)">Mechanical Engineer • Maker • Problem-solver</div>
        </div>
      </div>
      <nav>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <section class="hero">
      <div class="card intro">
        <h1>Hi — I’m [Your Name].</h1>
        <p>I design and build mechanical systems with a focus on manufacturability and real-world testing. I love prototyping, CAD, and turning ideas into reliable hardware.</p>
        <div class="cta">
          <a class="btn" href="#projects">See projects</a>
          <a class="ghost" href="#contact">Get in touch</a>
        </div>

        <div class="projects card" id="projects" style="margin-top:18px">
          <h3>Selected projects</h3>
          <div class="grid">
            <article class="proj">
              <h4>Lap Time Tracker</h4>
              <p>Arduino-based lap timing device with high-accuracy sensors and data logging.</p>
              <div class="tags"><span class="tag">C++</span><span class="tag">Arduino</span><span class="tag">Embedded</span></div>
            </article>

            <article class="proj">
              <h4>Telemetry Dashboard</h4>
              <p>Real-time telemetry visualization for launch simulations using Python and WebSocket streams.</p>
              <div class="tags"><span class="tag">Python</span><span class="tag">Realtime</span></div>
            </article>

            <article class="proj">
              <h4>Wind Turbine Blade</h4>
              <p>Composite blade prototype optimized for additive manufacturing and structural performance.</p>
              <div class="tags"><span class="tag">Composites</span><span class="tag">FEA</span></div>
            </article>

          </div>
        </div>

      </div>

      <aside class="profile card">
        <div class="avatar">[Your Photo]</div>
        <div class="meta">
          <h3>[Your Name]</h3>
          <p>Mechanical Engineering • UTD — Graduating May 2026</p>
        </div>

        <div class="card" style="width:100%; text-align:left">
          <h4 style="margin:0 0 8px 0">Skills</h4>
          <div class="skills" id="skills">
            <span class="skill">CAD (Creo / SolidWorks)</span>
            <span class="skill">MATLAB</span>
            <span class="skill">Manufacturing</span>
            <span class="skill">Embedded C++</span>
          </div>
        </div>

        <div style="width:100%">
          <a class="btn" href="mailto:you@example.com">you@example.com</a>
        </div>
      </aside>
    </section>

    <footer id="contact">
      <div class="card" style="display:inline-block; padding:18px; margin-bottom:12px">
        <strong>Contact</strong>
        <p style="margin:8px 0 0 0; color:var(--muted)">Email: <a href="mailto:you@example.com">you@example.com</a> • LinkedIn: <a href="#">linkedin.com/in/yourname</a></p>
      </div>

      <div>Built with ❤️ — customize this template and replace placeholder text and images with your own.</div>
    </footer>
  </div>
</body>
</html>
