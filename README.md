<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Página de Bienvenida</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #1e3c72, #2a5298);
      color: #f1f1f1;
    }
    h1 {
      font-size: 3rem;
      margin-bottom: 1rem;
      text-shadow: 2px 2px 6px rgba(0,0,0,0.4);
    }
    .fecha {
      font-size: 1.5rem;
      background: rgba(255,255,255,0.1);
      padding: 0.5rem 1rem;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }
  </style>
</head>
<body>
  <h1>Bienvenido</h1>
  <div class="fecha" id="fecha"></div>

  <script>
    // Obtener fecha actual
    const hoy = new Date();
    const opciones = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' };
    document.getElementById("fecha").textContent = hoy.toLocaleDateString("es-ES", opciones);
  </script>
</body>
</html>
