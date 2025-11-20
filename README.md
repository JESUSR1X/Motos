<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>MOTOLOCA</title>
  <style>
    body {
      margin: 0;
      font-family: "Segoe UI", Arial, sans-serif;
      background-color: #121212;
      color: #fff;
    }

    header {
      background: url("https://cdn-fastly.motor1.com/media/mgl/BbX6O/s3/kawasaki-ninja-h2r.jpg") no-repeat center center/cover;
      height: 90vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      position: relative;
    }

    header h1 {
      font-size: 4rem;
      letter-spacing: 2px;
      background: rgba(0, 0, 0, 0.6);
      padding: 1rem 2rem;
      border-radius: 15px;
      z-index: 2;
    }

    /* Contenedor del visor 360 */
    .viewer360 {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      height: 60%;
      background-color: rgba(0, 0, 0, 0.7);
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .viewer360 iframe {
      width: 80%;
      height: 90%;
      border: none;
      border-radius: 10px;
    }

    nav {
      display: flex;
      justify-content: center;
      background-color: #1e1e1e;
      padding: 1rem;
      gap: 2rem;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #bbb;
    }

    .motos {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
      padding: 3rem;
    }

    .moto {
      text-align: center;
      cursor: pointer;
      transition: transform 0.3s ease;
    }

    .moto:hover {
      transform: scale(1.05);
    }

    .moto img {
      width: 100%;
      border-radius: 10px;
    }

    .moto h2 {
      margin-top: 1rem;
    }

    footer {
      text-align: center;
      padding: 2rem;
      background-color: #1e1e1e;
    }

    .social {
      margin-top: 1rem;
      display: flex;
      justify-content: center;
      gap: 1rem;
    }

    .social a {
      color: white;
      font-size: 1.5rem;
      text-decoration: none;
    }

    /* MODAL */
    .modal {
      display: none;
      position: fixed;
      z-index: 999;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.8);
      justify-content: center;
      align-items: center;
    }

    .modal-content {
      background: #1e1e1e;
      padding: 2rem;
      border-radius: 10px;
      max-width: 700px;
      text-align: center;
      color: white;
      animation: fadeIn 0.5s ease forwards;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .modal-content img {
      width: 100%;
      border-radius: 10px;
      margin-bottom: 1rem;
    }

    .close {
      position: absolute;
      top: 20px;
      right: 30px;
      color: white;
      font-size: 2rem;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <nav>
    <a href="#inicio">Inicio</a>
    <a href="#motos">Motos</a>
    <a href="#quienes">Quiénes Somos</a>
    <a href="#ubicacion" id="ubicacion">Ubicación</a>
    <a href="#" id="contacto">Contacto</a>
  </nav>

  <header id="inicio">
    <h1>MOTOLOCA</h1>
    <div class="viewer360">
      <iframe src="https://sketchfab.com/models/8ce68b33d1d44cb3a23e06a303be9bdf/embed?autostart=1&ui_infos=0&ui_controls=1&ui_stop=0" allow="autoplay; fullscreen; xr-spatial-tracking" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
    </div>
  </header>

  <section id="motos" class="motos">
    <!-- (Se mantiene igual la sección de motos y modales del código anterior) -->
  </section>

  <section id="quienes" style="padding:3rem; text-align:center;">
    <h2>Quiénes Somos</h2>
    <p>En MOTOLOCA somos apasionados por la velocidad, la innovación y el estilo. Nos especializamos en motos deportivas de alto rendimiento con los últimos avances tecnológicos.</p>
  </section>

  <footer>
    <p>© 2025 MOTOLOCA | Todos los derechos reservados</p>
    <div class="social">
      <a href="https://www.instagram.com/" target="_blank">📸</a>
      <a href="https://www.facebook.com/" target="_blank">📘</a>
      <a href="https://x.com/" target="_blank">🐦</a>
    </div>
  </footer>

  <script>
    // Script igual que en el código anterior
  </script>
</body>
</html>
