# elegante-03
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Video de Fondo Adaptable</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow: hidden; /* Evita barras de desplazamiento innecesarias */
            font-family: sans-serif;
            color: white;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.7); /* Sombra para mejor legibilidad del texto */
        }
        #video-background {
            position: fixed;
            right: 0;
            bottom: 0;
            min-width: 100%;
            min-height: 100%;
            width: auto;
            height: auto;
            z-index: -100; /* Lo coloca detrás de todo el contenido */
            background-size: cover;
        }
        .overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.4); /* Capa semitransparente para oscurecer el video */
            z-index: 0;
        }
        .content {
            position: relative;
            z-index: 1; /* Asegura que el contenido esté sobre el video */
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            text-align: center;
            padding: 20px;
        }
        .content h1 {
            font-size: 3em;
            margin: 0;
        }
        .content p {
            font-size: 1.2em;
        }
    </style>
</head>
<body>
    <video id="video-background" autoplay muted loop>
        <source src="vip 02.mp4" type="video/mp4">
        Tu navegador no soporta el video.
    </video>
    <div class="overlay"></div>
    <div class="content">
        <h1>Tu Título Aquí</h1>
        <p>Este es el texto que se superpone al video de fondo.</p>
    </div>
</body>
</html>
