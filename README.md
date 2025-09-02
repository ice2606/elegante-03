# elegante-03
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
        <h1></h1>
        <p></p>
    </div>
</body>
</html>


<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Detalle del Producto</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #f4f4f4;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .product-card {
            max-width: 500px;
            width: 100%;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            margin-bottom: 20px;
            text-align: center;
        }
        .product-image {
            width: 100%;
            height: auto;
            display: block;
        }
        .product-content {
            padding: 20px;
        }
        .product-content h1 {
            margin-top: 0;
            font-size: 2em;
        }
        .product-content p {
            color: #555;
            line-height: 1.6;
            margin-bottom: 20px;
        }
        .whatsapp-button, .back-button {
            display: inline-block;
            width: 100%;
            padding: 12px 20px;
            text-decoration: none;
            color: white;
            font-weight: bold;
            border-radius: 5px;
            transition: background-color 0.3s ease;
            box-sizing: border-box; /* Asegura que el padding no afecte el ancho total */
            text-align: center;
        }
        .whatsapp-button {
            background-color: #25D366; /* Verde de WhatsApp */
            margin-bottom: 10px;
        }
        .whatsapp-button:hover {
            background-color: #128C7E;
        }
        .back-button {
            background-color: #333; /* Gris oscuro para el botón de atrás */
        }
        .back-button:hover {
            background-color: #555;
        }
        @media (min-width: 600px) {
            .whatsapp-button, .back-button {
                width: auto;
                padding-left: 30px;
                padding-right: 30px;
            }
        }
    </style>
</head>
<body>
    <div class="product-card">
        <img src="https://via.placeholder.com/500" alt="Imagen del producto" class="product-image">
        <div class="product-content">
            <h1>Nombre del Producto</h1>
            <p>
                Esta es una descripción detallada del producto. Aquí puedes explicar sus características, beneficios y por qué es la mejor opción.
                La información se ajustará automáticamente a cualquier pantalla, desde móviles pequeños hasta tabletas grandes.
            </p>
            <a href="https://wa.me/numerodetelefono?text=Hola,%20estoy%20interesado%20en%20el%20producto%20'Nombre%20del%20Producto'" class="whatsapp-button" target="_blank">
                Contactar por WhatsApp
            </a>
        </div>
    </div>
    <a href="https://ice2606.github.io/elegante-02/" class="back-button">
        Ir atrás
    </a>

</body>
</html>
