<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para el Amor de Mi Vida ❤️</title>
    <style>
        /* Estilos generales */
        body {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #ff9a9e 0%, #fad0c4 100%);
            color: #fff;
            overflow-x: hidden;
            text-align: center;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }

        h1 {
            font-size: 3em;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
            animation: pulse 2s infinite;
        }

        p {
            font-size: 1.2em;
            line-height: 1.6;
        }

        /* Corazones animados */
        .heart {
            position: absolute;
            width: 30px;
            height: 30px;
            background-color: #ff4d6d;
            transform: rotate(45deg);
            animation: float 6s ease-in-out infinite;
            opacity: 0.7;
        }

        .heart:before, .heart:after {
            content: "";
            position: absolute;
            width: 30px;
            height: 30px;
            background-color: #ff4d6d;
            border-radius: 50%;
        }

        .heart:before {
            top: -15px;
            left: 0;
        }

        .heart:after {
            top: 0;
            left: -15px;
        }

        /* Botón con efecto */
        .btn {
            display: inline-block;
            padding: 12px 24px;
            background: #ff4d6d;
            color: white;
            border: none;
            border-radius: 50px;
            font-size: 1.2em;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            margin-top: 20px;
        }

        .btn:hover {
            transform: scale(1.1);
            background: #ff758f;
        }

        /* Efecto de confeti */
        .confetti {
            position: fixed;
            width: 10px;
            height: 10px;
            background-color: #f00;
            opacity: 0.7;
            animation: confetti-fall 5s linear infinite;
        }

        /* Animaciones */
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        @keyframes float {
            0% { transform: rotate(45deg) translateY(0) translateX(0); }
            50% { transform: rotate(45deg) translateY(-20px) translateX(10px); }
            100% { transform: rotate(45deg) translateY(0) translateX(0); }
        }

        @keyframes confetti-fall {
            0% { transform: translateY(-100vh) rotate(0deg); opacity: 1; }
            100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
        }

        /* Mensaje oculto */
        #secret-message {
            display: none;
            margin-top: 30px;
            font-size: 1.5em;
            color: #ffeb3b;
            text-shadow: 0 0 5px rgba(0, 0, 0, 0.5);
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>❤️ Para Ti, Mi Amor ❤️</h1>
        <p>En cada latido de mi corazón, hay un recuerdo tuyo.</p>
        <p>Eres la razón por la que creo en el amor a primera vista, en los finales felices y en la magia.</p>
        <p>Hoy y siempre, estaré a tu lado.</p>
        
        <button class="btn" id="love-btn">Haz Clic Si Me Amas ❤️</button>
        
        <div id="secret-message">
            ¡Sabía que dirías que sí! Te amo más que a nada en este mundo. 💖
        </div>
    </div>

    <!-- Corazones flotantes -->
    <div id="hearts-container"></div>

    <script>
        // Crear corazones flotantes
        function createHearts() {
            const container = document.getElementById('hearts-container');
            for (let i = 0; i < 15; i++) {
                const heart = document.createElement('div');
                heart.classList.add('heart');
                heart.style.left = Math.random() * 100 + 'vw';
                heart.style.top = Math.random() * 100 + 'vh';
                heart.style.animationDelay = Math.random() * 5 + 's';
                container.appendChild(heart);
            }
        }

        // Crear confeti
        function createConfetti() {
            const colors = ['#ff4d6d', '#ffeb3b', '#4caf50', '#2196f3', '#9c27b0'];
            const container = document.body;
            for (let i = 0; i < 100; i++) {
                const confetti = document.createElement('div');
                confetti.classList.add('confetti');
                confetti.style.left = Math.random() * 100 + 'vw';
                confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
                confetti.style.animationDuration = Math.random() * 3 + 2 + 's';
                container.appendChild(confetti);
            }
        }

        // Mostrar mensaje secreto al hacer clic
        document.getElementById('love-btn').addEventListener('click', function() {
            document.getElementById('secret-message').style.display = 'block';
            createConfetti();
            this.style.display = 'none';
        });

        // Inicializar corazones al cargar la página
        window.onload = createHearts;
    </script>
</body>
</html>
