<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¡Feliz Día del Maestro! - Panchito</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Montserrat:wght@400;700&display=swap');
        
        body {
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            font-family: 'Montserrat', sans-serif;
            overflow-x: hidden;
            color: #333;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
            text-align: center;
        }
        
        h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 3.5rem;
            color: #e74c3c;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
            animation: pulse 2s infinite;
        }
        
        h2 {
            color: #2c3e50;
            margin-top: 0;
            font-size: 1.8rem;
        }
        
        .card {
            background: white;
            border-radius: 15px;
            padding: 30px;
            margin: 30px 0;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            position: relative;
            overflow: hidden;
            transition: transform 0.3s;
        }
        
        .card:hover {
            transform: translateY(-10px);
        }
        
        .card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 10px;
            background: linear-gradient(90deg, #e74c3c, #3498db, #2ecc71, #f1c40f, #9b59b6);
        }
        
        p {
            font-size: 1.2rem;
            line-height: 1.6;
            margin-bottom: 20px;
        }
        
        .quote {
            font-style: italic;
            font-size: 1.4rem;
            color: #7f8c8d;
            margin: 40px 0;
            position: relative;
        }
        
        .quote::before, .quote::after {
            content: '"';
            font-size: 2rem;
            color: #e74c3c;
        }
        
        .teachers {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin: 40px 0;
        }
        
        .teacher {
            background: white;
            border-radius: 10px;
            padding: 15px;
            width: 150px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s;
        }
        
        .teacher:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }
        
        .teacher-icon {
            font-size: 3rem;
            color: #3498db;
            margin-bottom: 10px;
        }
        
        .thank-you {
            font-size: 2rem;
            color: #e74c3c;
            margin: 50px 0;
            animation: float 3s ease-in-out infinite;
        }
        
        .signature {
            font-family: 'Dancing Script', cursive;
            font-size: 2rem;
            color: #2c3e50;
            margin-top: 50px;
        }
        
        .confetti {
            position: fixed;
            width: 10px;
            height: 10px;
            background-color: #f00;
            opacity: 0;
            animation: confetti 5s ease-in-out infinite;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
        
        @keyframes confetti {
            0% { 
                transform: translateY(0) rotate(0deg);
                opacity: 1;
            }
            100% { 
                transform: translateY(100vh) rotate(720deg);
                opacity: 0;
            }
        }
        
        .heart {
            color: #e74c3c;
            animation: heartbeat 1.5s infinite;
            display: inline-block;
        }
        
        @keyframes heartbeat {
            0% { transform: scale(1); }
            25% { transform: scale(1.1); }
            50% { transform: scale(1); }
            75% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }
        
        .video-container {
            position: relative;
            padding-bottom: 56.25%; /* 16:9 aspect ratio */
            height: 0;
            overflow: hidden;
            margin: 40px 0;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }
        
        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
        }
        
        .video-message {
            margin-top: 20px;
            font-size: 1.1rem;
            color: #7f8c8d;
        }
        
        .song-info {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 10px;
            margin: 20px 0;
            font-style: italic;
        }
        
        .play-button {
            background: #e74c3c;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 50px;
            font-size: 1.1rem;
            cursor: pointer;
            margin: 15px 0;
            transition: all 0.3s;
        }
        
        .play-button:hover {
            background: #c0392b;
            transform: scale(1.05);
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>¡Feliz Día del Maestro!</h1>
        <h2>Para todos los profesores de la Panchito</h2>
        
        <div class="card">
            <p>Queridos profesores,</p>
            <p>Hoy es un día especial para reconocer su invaluable labor. Cada día, con paciencia y dedicación, moldean no solo mentes sino también corazones.</p>
            
            <div class="quote">
                Un buen maestro puede inspirar esperanza, encender la imaginación e inculcar un amor por el aprendizaje.
            </div>
            
            <p>En la Panchito, sabemos que ustedes son esos maestros excepcionales que dejan huella en la vida de sus estudiantes.</p>
        </div>
        
        <div class="teachers">
            <div class="teacher">
                <div class="teacher-icon">📚</div>
                <h3>Profes de Letras</h3>
                <p>Gracias por enseñarnos a expresarnos</p>
            </div>
            
            <div class="teacher">
                <div class="teacher-icon">🧮</div>
                <h3>Profes de Ciencias</h3>
                <p>Gracias por mostrarnos el mundo</p>
            </div>
            
            <div class="teacher">
                <div class="teacher-icon">🎨</div>
                <h3>Profes de Arte</h3>
                <p>Gracias por despertar nuestra creatividad</p>
            </div>
            
            <div class="teacher">
                <div class="teacher-icon">⚽</div>
                <h3>Profes de Deporte</h3>
                <p>Gracias por enseñarnos disciplina</p>
            </div>
        </div>
        
        <div class="card">
            <h2>Homenaje Musical</h2>
            <p>Hemos preparado este emotivo tema musical como tributo a su labor incansable:</p>
            
            <div class="song-info">
                "Gracias Maestro" - Willie Rosario<br>
                Una canción que expresa el agradecimiento a todos los maestros
            </div>
            
            <!-- Video musical específico -->
            <div class="video-container">
                <iframe id="teacherVideo" src="https://www.youtube.com/embed/NrAFXt7ML_8?si=O3zJip_hx2ui8OZF&enablejsapi=1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
            
            
            <p class="video-message">Dedíquense estos minutos de música a ustedes, queridos maestros</p>
            
            <p>Este homenaje musical es solo una pequeña muestra de nuestro inmenso agradecimiento por todo lo que hacen.</p>
        </div>
        
        <div class="thank-you">
            ¡GRACIAS POR TODO! <span class="heart">❤️</span>
        </div>
        
        <div class="signature">
            Con cariño,<br>
            La comunidad de la Panchito
        </div>
    </div>
    
    <script>
        // Create confetti
        function createConfetti() {
            const colors = ['#e74c3c', '#3498db', '#2ecc71', '#f1c40f', #9b59b6'];
            
            for (let i = 0; i < 100; i++) {
                const confetti = document.createElement('div');
                confetti.className = 'confetti';
                confetti.style.left = Math.random() * 100 + 'vw';
                confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
                confetti.style.width = Math.random() * 10 + 5 + 'px';
                confetti.style.height = Math.random() * 10 + 5 + 'px';
                confetti.style.animationDuration = Math.random() * 3 + 2 + 's';
                confetti.style.animationDelay = Math.random() * 5 + 's';
                document.body.appendChild(confetti);
            }
        }
        
        // YouTube API
        let player;
        function onYouTubeIframeAPIReady() {
            player = new YT.Player('teacherVideo', {
                events: {
                    'onReady': onPlayerReady
                }
            });
        }
        
        function onPlayerReady(event) {
            // Player is ready
        }
        
        function playVideo() {
            if (player) {
                player.playVideo();
            }
        }
        
        // Create interactive elements
        document.addEventListener('DOMContentLoaded', function() {
            createConfetti();
            
            // Load YouTube API
            const tag = document.createElement('script');
            tag.src = "https://www.youtube.com/iframe_api";
            const firstScriptTag = document.getElementsByTagName('script')[0];
            firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);
            
            // Add click effect for cards
            const cards = document.querySelectorAll('.card');
            cards.forEach(card => {
                card.addEventListener('click', function() {
                    this.style.transform = 'scale(0.98)';
                    setTimeout(() => {
                        this.style.transform = '';
                    }, 200);
                });
            });
            
            // Add message when clicking on teachers
            const teachers = document.querySelectorAll('.teacher');
            teachers.forEach(teacher => {
                teacher.addEventListener('click', function() {
                    const subject = this.querySelector('h3').textContent;
                    alert(`¡Gracias profesores de ${subject} por su dedicación!`);
                });
            });
        });
    </script>
</body>
</html>