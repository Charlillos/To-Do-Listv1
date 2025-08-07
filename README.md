# To-Do-Listv1
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Página Principal</title>
  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Delicata&family=Inter:wght@400;600&family=Saira&display=swap" rel="stylesheet">

  <style>
.fade-in {
  opacity: 5;
  animation: fadeIn 2.5s ease-in forwards;
}

@keyframes fadeIn {
  to {
    opacity: 1;
  }
}
    body {
      margin: 0;
      font-family: -apple-system, BlinkMacSystemFont, sans-serif;
      overflow: hidden;
      background: linear-gradient(315deg, rgba(101,0,94,1) 3%, rgba(60,132,206,1) 38%, rgba(48,238,226,1) 68%, rgba(255,25,25,1) 98%);
      animation: gradient 15s ease infinite;
      background-size: 400% 400%;
      background-attachment: fixed;
      height: 100vh;
      position: relative;
    }

    @keyframes gradient {
      0% { background-position: 0% 0%; }
      50% { background-position: 100% 100%; }
      100% { background-position: 0% 0%; }
    }

    .wave {
      background: rgb(255 255 255 / 25%);
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
      opacity: 0.8;
    }

    .wave:nth-of-type(3) {
      bottom: -2.5em;
      animation: wave 20s -1s reverse infinite;
      opacity: 0.9;
    }

    @keyframes wave {
      2% { transform: translateX(1); }
      25% { transform: translateX(-25%); }
      50% { transform: translateX(-50%); }
      75% { transform: translateX(-25%); }
      100% { transform: translateX(1); }
    }

    .contenido {
      position: relative;
      z-index: 1;
      height: 100%;
      width: 100%;
      padding: 2rem;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
    }

    h1 {
      font-family: "Saira", sans-serif;
      font-weight: 800;
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    p {
      font-family: "Saira", sans-serif;
      font-weight: 400;
      font-size: 1.2rem;
      max-width: 700px;
      margin-bottom: 1.5rem;
    }

    button {
      font-family: 'Inter', sans-serif;
      font-size: 1rem;
      padding: 12px 24px;
      margin: 0.5rem;
      border: none;
      border-radius: 8px;
      background: white;
      color: black;
      cursor: pointer;
      transition: transform 0.3s, background-color 0.3s;
    }

    button:hover {
      background: #ff7eb3;
      transform: scale(1.05);
    }
  </style>
</head>
<body>

  <!-- Olas animadas -->
  <div class="wave"></div>
  <div class="wave"></div>
  <div class="wave"></div>

  <!-- Contenido centrado -->
  <div class="contenido">
    <h1 class="fade-in">BIENVENIDOS A NUESTRO SITIO DE GESTIÓN DE TAREAS Y DEBERES</h1>
    <p>Este es un sitio donde le podemos ayudar a gestionar, administrar, guardar y mostrar las tareas o deberes que usted tiene que realizar para x fecha y pueda organizar mejor su tiempo para que ocupe lo necesario para cada tarea.</p>
    
><button>Aprenda a usarlo</button>
    
    <p>En dado caso usted ya sabe cómo utilizar este sitio web, entonces puede darle clic aquí</p>
    
   <button>Inicie su planificación aquí</button>
  </div>

</body>
</html>

