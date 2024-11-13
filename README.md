<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>La Antigua Roma</title>
    <style>
        /* Estilos básicos para la página */
        body {
            background-image: url('https://curiosidades.com/wp-content/uploads/2023/07/image-3.png'); /* Imagen de fondo temática */
            background-size: cover;
            background-attachment: fixed;
            font-family: Arial, sans-serif;
            color: #333;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: rgba(0, 0, 0, 0.7); /* Fondo oscuro para contraste */
            color: #f4d03f; /* Dorado para destacar */
            padding: 1em;
            text-align: center;
        }

        .marquee {
            background-color: rgba(255, 255, 255, 0.8);
            color: #333;
            font-weight: bold;
            padding: 0.5em;
            text-align: center;
            overflow: hidden;
            white-space: nowrap;
        }

        .container {
            padding: 2em;
            text-align: center;
            background-color: rgba(255, 255, 255, 0.8);
            margin: 20px;
            border-radius: 8px;
        }

        .container img {
            max-width: 100%;
            height: auto;
            border: 2px solid #f4d03f;
            border-radius: 8px;
        }
    </style>
</head>
<body>

    <!-- Encabezado de la página -->
    <header>
        <h1>Descubre la Antigua Roma</h1>
    </header>

    <!-- Marquesina con texto -->
    <div class="marquee" id="marquee-text">
        La cuna de la civilización romana, sus logros y su legado en la historia.
    </div>

    <!-- Contenido principal de la página -->
    <div class="container">
        <!-- Imagen de la Antigua Roma -->
        <img src="https://curiosidades.com/wp-content/uploads/2023/07/image-3.png" alt="Imagen de la Antigua Roma">

        <!-- Reseña de la página -->
        <p>
            La Antigua Roma fue una de las civilizaciones más influyentes en la historia de la humanidad. Desde su fundación en el siglo VIII a.C., Roma dejó un legado monumental en arquitectura, derecho, gobierno y cultura que ha perdurado hasta nuestros días. A través de sus logros en ingeniería, arte y organización social, el Imperio Romano estableció las bases de muchas sociedades modernas. En esta página, exploraremos algunos de los aspectos más fascinantes de su cultura, costumbres y contribuciones.
        </p>
    </div>

    <!-- JavaScript para la marquesina -->
    <script>
        // Selecciona el elemento de la marquesina
        const marqueeText = document.getElementById("marquee-text");

        // Configura el movimiento de desplazamiento de la marquesina
        function scrollMarquee() {
            marqueeText.style.transition = "transform 10s linear";
            marqueeText.style.transform = "translateX(-100%)";
        }

        // Reinicia la posición después del desplazamiento
        marqueeText.addEventListener("transitionend", () => {
            marqueeText.style.transition = "none";
            marqueeText.style.transform = "translateX(100%)";
            // Inicia el desplazamiento después de un pequeño retraso
            setTimeout(scrollMarquee, 100);
        });

        // Inicia el desplazamiento la primera vez
        scrollMarquee();
    </script>

</body>
</html>
