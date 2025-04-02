# Proyecto: Mis Trabajos Universitarios

Este proyecto muestra una página web donde presento mis trabajos universitarios, incluyendo detalles sobre mi carrera, materia, profesor, entre otros.

## Código de la Página Principal (index.html)

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mis Trabajos Universitarios</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <style>
        /* Estilos generales */
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
            background: linear-gradient(to right, #4C6D87, #1f3b4f);
        }

        header {
            text-align: center;
            color: white;
            padding: 50px 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            background-color: rgba(31, 59, 79, 0.9);
            border-bottom: 5px solid #FFD700;
        }

        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        header p {
            font-size: 1.5em;
            margin: 10px 0;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
            text-align: center;
            background-color: rgba(0, 0, 0, 0.8);
            margin: 0;
        }

        nav ul li {
            display: inline;
            margin: 0 30px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            font-size: 1.2em;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        nav ul li a:hover {
            color: #FFD700;
            transition: all 0.3s ease-in-out;
        }

        section {
            margin: 40px;
            padding: 30px;
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        section h2 {
            font-size: 2.5em;
            color: #1f3b4f;
            margin-bottom: 20px;
            text-align: center;
            text-transform: uppercase;
        }

        section p {
            font-size: 1.2em;
            line-height: 1.6;
            margin-bottom: 20px;
        }

        footer {
            text-align: center;
            padding: 20px;
            background-color: #1f3b4f;
            color: white;
            font-size: 1.1em;
        }

        /* Estilos del carrusel */
        .carousel-container {
            display: flex;
            overflow: hidden;
            width: 100%;
            justify-content: center;
            align-items: center;
            margin-top: 40px;
        }

        .carousel-item {
            flex: 0 0 100%;
            text-align: center;
            display: none;
            animation: slideIn 1s ease-in-out;
        }

        .carousel-item.active {
            display: block;
        }

        @keyframes slideIn {
            0% { opacity: 0; transform: translateY(30px); }
            100% { opacity: 1; transform: translateY(0); }
        }

        /* Estilos para la imagen personal */
        .foto-personal {
            width: 150px;
            height: 150px;
            border-radius: 50%; /* Hace la imagen redonda */
            margin: 0 auto;
            border: 4px solid #FFD700; /* Borde dorado */
            object-fit: cover; /* Asegura que la imagen se ajuste bien */
        }

        /* Para los botones y enlaces */
        .trabajo a {
            color: #4C6D87;
            font-size: 1.1em;
            padding: 10px 20px;
            text-decoration: none;
            border: 2px solid #4C6D87;
            border-radius: 5px;
            background-color: #f7f7f7;
            transition: all 0.3s ease;
        }

        .trabajo a:hover {
            background-color: #4C6D87;
            color: white;
            border-color: #1f3b4f;
        }
    </style>
</head>
<body>
    <header>
        <h1>Mis Trabajos Universitarios</h1>
        <p>Explora mis proyectos y trabajos realizados durante mi carrera en Ingeniería en Redes y Telecomunicaciones.</p>
    </header>

    <nav>
        <ul>
            <li><a href="#informacion">Información Personal</a></li>
            <li><a href="#trabajos">Mis Trabajos</a></li>
            <li><a href="#contacto">Contacto</a></li>
        </ul>
    </nav>

    <!-- Sección de Información Personal (Carrusel) -->
    <section id="informacion">
        <h2>Información Personal</h2>
        <div class="carousel-container">
            <div class="carousel-item active">
                <!-- Imagen Personal -->
                <img src="imagenes/foto1.jpeg" alt="Foto de Luis Miguel Ramirez Leon" class="foto-personal">
                <h3>Mi Información</h3>
                <p><strong>Nombre:</strong> Luis Miguel Ramirez Leon</p>
                <p><strong>Carrera:</strong> Ingeniería en Redes y Telecomunicaciones</p>
                <p><strong>Materia:</strong> Sistemas Telemáticos</p>
                <p><strong>Profesor:</strong> Luis Rey Lara Gonzales</p>
                <p><strong>Matrícula:</strong> 321030370</p>
                <p><strong>Correo Electrónico:</strong> <a href="mailto:321030370@upjr.edu.mx">321030370@upjr.edu.mx</a></p>
            </div>
        </div>
    </section>

    <section id="trabajos">
        <h2>Mis Trabajos</h2>
        <div class="trabajo">
            <h3>Trabajo 1: Introducción a Oracle</h3>
            <p>Oracle Cloud es relevante porque permite implementar y gestionar soluciones de comunicación, redes y bases de datos, que son fundamentales en la transmisión de datos y la administración de sistemas distribuidos.</p>
            <a href="https://github.com/Luismi14/Oracle" target="_blank">Ver más en GitHub</a>
        </div>
        <div class="trabajo">
            <h3>Trabajo 2: Investigación sobre Inteligencia Artificial</h3>
            <p>Descripción breve del proyecto.</p>
            <a href="https://github.com/Luismi14/proyecto2" target="_blank">Ver más en GitHub</a>
        </div>
    </section>

    <section id="contacto">
        <h2>Contacto</h2>
        <p>Si deseas ponerte en contacto conmigo, puedes enviarme un correo a <a href="mailto:321030370@upjr.edu.mx">321030370@upjr.edu.mx</a>.</p>
    </section>

    <footer>
        <p>&copy; 2025 Mis Trabajos Universitarios</p>
    </footer>

    <script>
        let currentIndex = 0;
        const items = document.querySelectorAll('.carousel-item');
        
        function showNext() {
            items[currentIndex].classList.remove('active');
            currentIndex = (currentIndex + 1) % items.length;
            items[currentIndex].classList.add('active');
        }

        setInterval(showNext, 5000);
    </script>
</body>
</html>
