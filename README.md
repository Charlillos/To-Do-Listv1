# To-Do-Listv1
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <title>Página Principal</title>
   <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Delicata&family=Inter:wght@400;600&family=Saira&display=swap" rel="stylesheet">
  <style>
    /* Animación fade-in */
    .fade-in {
      opacity: 0;
      animation: fadeIn 2.5s ease-in forwards;
    }
    @keyframes fadeIn {
      to { opacity: 1; }
    }

    body {
      margin: 0;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
        Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
      overflow: hidden;
      background: linear-gradient(315deg, #65005e 3%, #3c84ce 38%, #30eee2 68%, #ff1919 98%);
      animation: gradient 15s ease infinite;
      background-size: 400% 400%;
      background-attachment: fixed;
      height: 100vh;
      position: relative;
      color: white;
      text-align: center;
      padding: 2rem;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    @keyframes gradient {
      0% { background-position: 0% 0%; }
      50% { background-position: 100% 100%; }
      100% { background-position: 0% 0%; }
    }

    .wave {
      background: rgba(255, 255, 255, 0.25);
      border-radius: 1000% 1000% 0 0;
      position: fixed;
      width: 200%;
      height: 12em;
      animation: wave 10s -3s linear infinite;
      transform: translate3d(0, 0, 0);
      opacity: 0.8;
      bottom: 0;
      left: 0;
      z-index: 0;
    }
    .wave:nth-of-type(2) {
      bottom: -1.25em;
      animation: wave 18s linear reverse infinite;
    }
    .wave:nth-of-type(3) {
      bottom: -2.5em;
      animation: wave 20s -1s reverse infinite;
    }
    @keyframes wave {
      2% { transform: translateX(1); }
      25% { transform: translateX(-25%); }
      50% { transform: translateX(-50%); }
      75% { transform: translateX(-25%); }
      100% { transform: translateX(1); }
    }

    h1 {
      font-weight: 800;
      font-size: 2.5rem;
      margin-bottom: 1rem;
      font-family: system-ui, sans-serif;
    }

    p {
      font-weight: 400;
      font-size: 1.2rem;
      max-width: 700px;
      margin-bottom: 1.5rem;
      font-family: system-ui, sans-serif;
    }

    button {
      font-size: 1rem;
      padding: 12px 24px;
      margin: 0.5rem;
      border: none;
      border-radius: 8px;
      background: white;
      color: black;
      cursor: pointer;
      transition: transform 0.3s, background-color 0.3s;
      font-family: system-ui, sans-serif;
    }
    button:hover {
      background: #ff7eb3;
      transform: scale(1.05);
    }
  </style>
</head>
<body>
  <div class="wave"></div>
  <div class="wave"></div>
  <div class="wave"></div>

  <h1 class="fade-in">BIENVENIDOS A NUESTRO SITIO DE GESTIÓN DE TAREAS Y DEBERES</h1>
  <p>Este es un sitio donde le podemos ayudar a gestionar, administrar, guardar y mostrar las tareas o deberes que usted tiene que realizar para x fecha y pueda organizar mejor su tiempo para que ocupe lo necesario para cada tarea.</p>

  <!-- Cambia los nombres de archivos según tu proyecto y asegúrate que estén subidos -->
  <p>En dado caso usted ya sabe cómo utilizar este sitio web, entonces puede darle clic aquí</p>
</body>
</html>
