
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amor da minha vida, Luana Ferreira dos Santos</title>
    <link href="https://fonts.googleapis.com/css2?family=Bright+Sunshine:wght@400&family=Dancing+Script:wght@400&family=Great+Vibes&family=Lobster&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            background-color: #000;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: 'Arial', sans-serif;
            color: #fff;
            text-align: center;
            overflow: hidden;
        }
        .container {
            position: relative;
            z-index: 1;
        }
        .heart {
            position: relative;
            width: 120px;
            height: 120px;
            background-color: red;
            transform: rotate(-45deg);
            animation: pulse 1.5s infinite;
            margin: 0 auto;
        }
        .heart::before,
        .heart::after {
            content: "";
            position: absolute;
            width: 120px;
            height: 120px;
            background-color: red;
            border-radius: 50%;
        }
        .heart::before {
            top: -60px;
            left: 0;
        }
        .heart::after {
            left: 60px;
            top: 0;
        }
        .heart-text {
            position: absolute;
            top: -90px;
            left: 50%;
            transform: translateX(-50%);
            color: #ff97d9;
            font-size: 24px;
            font-family: 'Lobster', cursive;
            text-shadow: 0 0 10px rgba(255, 151, 217, 0.8), 0 0 20px rgba(255, 151, 217, 0.6);
            font-weight: bold;
        }
        .message {
            margin-top: 160px;
            font-size: 24px;
            font-family: 'Great Vibes', cursive;
        }
        .sparkles {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: 0;
        }
        .sparkle {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: rgba(255, 151, 217, 0.5);
            transform: rotate(-45deg);
            animation: sparkle 3s linear infinite;
        }
        .sparkle::before,
        .sparkle::after {
            content: "";
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: rgba(255, 151, 217, 0.5);
            border-radius: 50%;
        }
        .sparkle::before {
            top: -10px;
            left: 0;
        }
        .sparkle::after {
            left: 10px;
            top: 0;
        }
        @keyframes pulse {
            0% {
                transform: scale(1) rotate(-45deg);
            }
            50% {
                transform: scale(1.1) rotate(-45deg);
            }
            100% {
                transform: scale(1) rotate(-45deg);
            }
        }
        @keyframes sparkle {
            0% {
                transform: translateY(0) scale(1);
                opacity: 0.8;
            }
            50% {
                opacity: 0;
            }
            100% {
                transform: translateY(-200px) scale(0);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <div class="sparkles">
        <div class="sparkle" style="top: 10%; left: 20%; animation-duration: 2s;"></div>
        <div class="sparkle" style="top: 30%; left: 50%; animation-duration: 3s;"></div>
        <div class="sparkle" style="top: 60%; left: 80%; animation-duration: 1.5s;"></div>
        <div class="sparkle" style="top: 80%; left: 40%; animation-duration: 2.5s;"></div>
        <div class="sparkle" style="top: 50%; left: 70%; animation-duration: 2s;"></div>
    </div>
    <div class="container">
        <div class="heart"></div>
        <div class="heart-text">EU TE AMO</div>
        <div class="message">
            Te amo meu amor, você é tudo que eu sempre quis. Feliz Aniversário para nós, você é tudo de bom.
        </div>
    </div>
</body>
</html>
