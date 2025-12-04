<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Bienvenido</title>
  <style>
    :root { --bg:#0f172a; --card:#111827; --text:#e5e7eb; --accent:#38bdf8; }
    *{box-sizing:border-box}
    body{
      margin:0; font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
      background: radial-gradient(900px 500px at 20% 0%, #1f2937 0%, var(--bg) 40%) fixed;
      color:var(--text); display:grid; min-height:100vh; place-items:center;
    }
    .card{
      width:min(720px, 92%); background:linear-gradient(180deg,#0b1220,var(--card));
      border:1px solid #1f2937; border-radius:16px; padding:2rem; text-align:center;
      box-shadow:0 18px 50px rgba(0,0,0,.35);
    }
    h1{margin:0 0 .5rem; font-size:clamp(2rem,4vw,3rem)}
    p{margin:.5rem 0 1.25rem; color:#cbd5e1; font-size:clamp(1rem,2.3vw,1.15rem)}
    .btn{
      display:inline-block; padding:.75rem 1.25rem; border-radius:12px;
      background:#0b1220; border:1px solid #1f2937; color:var(--text); text-decoration:none;
      transition:transform .08s ease, box-shadow .2s ease, border-color .2s ease;
    }
    .btn:hover{ border-color:var(--accent); box-shadow:0 10px 24px rgba(56,189,248,.25); transform:translateY(-1px) }
    .accent{ position:relative; display:inline-block }
    .accent::after{
      content:""; position:absolute; left:0; right:0; bottom:-8px; height:3px;
      background:linear-gradient(90deg,var(--accent),#a78bfa); border-radius:999px; opacity:.7;
    }
    footer{ margin-top:1rem; font-size:.9rem; color:#94a3b8 }
  </style>
</head>
<body>
  <main class="card">
    <h1><span class="accent">Bienvenido</span> a mi sitio</h1>
    <p>Gracias por visitar la página. Empieza a explorar y disfruta del contenido.</p>
    <a class="btn" href="#comenzar">Comenzar</a>
    <footer>HTML + CSS ligero, rápido y responsive.</footer>
  </main>
</body>
</html>
