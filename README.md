<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cartas del Destino</title>
    <style>
        body {
            background-color: pink;
            text-align: center;
            font-family: Arial, sans-serif;
        }
        h1 {
            color: #d63384;
        }
        .cartas {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 30px;
        }
        .carta {
            width: 150px;
            height: 200px;
            background-color: black;
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 20px;
            border-radius: 10px;
            cursor: pointer;
            transition: transform 0.5s;
        }
        .carta:hover {
            transform: scale(1.1);
        }
        .carta.abierta {
            background-color: white;
            color: black;
            font-size: 18px;
            padding: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <h1>¡Las Cartas del Destino para Keysi Rodríguez! ❤️</h1>
    <div class="cartas">
        <div class="carta" onclick="mostrarMensaje(this, 'Eres mi felicidad ❤️')"></div>
        <div class="carta" onclick="mostrarMensaje(this, 'Siempre estaré a tu lado 💖')"></div>
        <div class="carta" onclick="mostrarMensaje(this, 'Te amo con todo mi corazón mi ochita panzoncita❤️')"></div>
    </div>
    <script>
        function mostrarMensaje(carta, mensaje) {
            carta.classList.add('abierta');
            carta.innerHTML = mensaje;
        }
    </script>
    <p>Con amor, Carlos Hernández 💕</p>
</body>
</html>
