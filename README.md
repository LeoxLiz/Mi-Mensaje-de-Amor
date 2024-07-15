# Mi-Mensaje-de-Amor
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mensaje de Amor</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <div class="card" id="card">
            <div class="card-content" id="card-content">
                Ábreme
            </div>
        </div>
        <div class="letter" id="letter">
            <p>Para Liz, mi amor eterno:</p>
            <p>En el vasto universo de mi corazón, tú eres la estrella más brillante, el faro que ilumina mis noches y da sentido a mis días. Desde el momento en que tus ojos color café se cruzaron con los míos, supe que había encontrado el paisaje más hermoso del mundo en esos ojitos maravillosos. Cada mirada tuya es un recordatorio de que la belleza más pura reside en ti.</p>
            <p>Tu pelo, tan liso y hermoso, me enreda en un hechizo del que no quiero escapar. Cada hebra es un hilo de amor que me ata a ti, y no hay lugar en el que prefiera estar más que envuelto en tu esencia. Tu sonrisa, mi vida, es un sol que amanece en mi alma, desvaneciendo cualquier sombra de tristeza y llenando mi corazón de alegría y esperanza.</p>
            <p>Adoro tus gestos, tu forma de ser que me encanta más con cada día que pasa. Eres mi razón de existir, el motor que impulsa mi vida y me inspira a ser mejor, tanto como persona como el amor de tu vida. Contigo, quiero todo y más. No hay obstáculo, no hay desafío que pueda detenerme, porque mi amor por ti es más fuerte que cualquier adversidad.</p>
            <p>Prometo que nunca nos separaremos. Hoy, mañana y siempre, estaremos juntos. Te amo con cada fibra de mi ser, con todo mi corazón y alma. Eres mi mundo entero, y en cada estrella que veo en el cielo, encuentro tu hermosa cara reflejada, iluminando mis noches.</p>
            <p>Solo puedo pensar en el futuro que construiremos juntos, en todas las cosas tontas y cursis que prometo cumplir. Porque tú te mereces todo, y yo estoy dispuesto a darte todo. Aprecio cada segundo que paso contigo, cada momento en que reímos sin parar, cada instante en que simplemente estamos juntos.</p>
            <p>Gracias, mi amor, por hacerme tan feliz con solo escuchar tu voz, leer un mensaje, o simplemente imaginar tu preciosa carita. Eres mi felicidad, mi alegría, mi todo. Te amo muchísimo, Liz, más de lo que las palabras pueden expresar.</p>
            <p>Con todo mi amor,<br>Leo, el amor de tu eternidad</p>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>
body {
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #000;
    color: #fff;
    font-family: Arial, sans-serif;
}

.container {
    position: relative;
    text-align: center;
}

.card {
    width: 200px;
    height: 200px;
    background-color: red;
    border-radius: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 24px;
    cursor: pointer;
    animation: heartbeat 1s infinite;
}

.card-content {
    position: relative;
}

.card-content::before, .card-content::after {
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    background: radial-gradient(circle, rgba(255,255,255,0.3) 0%, rgba(255,255,255,0) 70%);
    animation: shimmer 2s infinite;
}

.letter {
    display: none;
    width: 80%;
    height: 80%;
    background-color: #fff;
    color: #000;
    padding: 20px;
    border-radius: 10px;
    text-align: left;
    overflow-y: auto;
}

@keyframes heartbeat {
    0%, 100% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.1);
    }
}

@keyframes shimmer {
    0% {
        opacity: 0.3;
    }
    50% {
        opacity: 1;
    }
    100% {
        opacity: 0.3;
    }
}
document.getElementById('card').addEventListener('click', function() {
    this.style.display = 'none';
    document.getElementById('letter').style.display = 'block';
});
