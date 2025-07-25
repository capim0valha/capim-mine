<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Entre no Discord - Experiência Animada</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Variáveis e estilos gerais */
        :root {
            --discord-primary: #5865F2;
            --discord-secondary: #7289DA;
            --discord-dark: #36393F;
            --discord-darker: #2F3136;
            --discord-light: #FFFFFF;
            --discord-accent: #EB459E;
            --discord-green: #57F287;
            --discord-yellow: #FEE75C;
            --discord-red: #ED4245;
            --discord-purple: #9B59B6;
            --discord-orange: #E67E22;
            
            --transition-speed: 0.3s;
            --animation-speed: 1s;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--discord-dark);
            color: var(--discord-light);
            overflow-x: hidden;
            perspective: 1000px;
        }
        
        /* Efeito de partículas no fundo */
        .particles-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            overflow: hidden;
        }
        
        .particle {
            position: absolute;
            border-radius: 50%;
            opacity: 0.5;
            animation: float-particle var(--animation-speed) infinite linear;
        }
        
        /* Container principal */
        .main-container {
            max-width: 100%;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 2rem;
            position: relative;
            z-index: 1;
            overflow: hidden;
        }
        
        /* Seção de boas-vindas */
        .welcome-section {
            text-align: center;
            margin-bottom: 3rem;
            opacity: 0;
            transform: translateY(50px);
            animation: fade-in-up 1.2s forwards;
        }
        
        .welcome-title {
            font-size: 4rem;
            font-weight: 800;
            margin-bottom: 1rem;
            color: var(--discord-light);
            text-shadow: 0 0 10px rgba(88, 101, 242, 0.8);
            position: relative;
            display: inline-block;
        }
        
        .welcome-title span {
            display: inline-block;
            animation: letter-bounce 2s infinite;
            animation-delay: calc(0.1s * var(--i));
        }
        
        .welcome-subtitle {
            font-size: 1.5rem;
            color: var(--discord-secondary);
            margin-bottom: 2rem;
            opacity: 0;
            animation: fade-in 1s forwards 0.5s;
        }
        
        /* Cartões de recursos */
        .features-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 2rem;
            margin-bottom: 3rem;
            perspective: 1000px;
        }
        
        .feature-card {
            background: rgba(47, 49, 54, 0.8);
            backdrop-filter: blur(10px);
            border-radius: 1rem;
            padding: 2rem;
            width: 300px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            text-align: center;
            transition: transform var(--transition-speed), box-shadow var(--transition-speed);
            opacity: 0;
            transform: translateY(50px) rotateX(10deg);
            animation: card-appear 0.8s forwards;
            animation-delay: calc(0.2s * var(--card-i));
            position: relative;
            overflow: hidden;
            border: 2px solid transparent;
        }
        
        .feature-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, 
                transparent, 
                rgba(88, 101, 242, 0.1), 
                transparent);
            transform: rotate(45deg);
            animation: shine 3s infinite;
        }
        
        .feature-card:hover {
            transform: translateY(-10px) rotateX(0deg);
            box-shadow: 0 15px 40px rgba(88, 101, 242, 0.4);
            border-color: var(--discord-secondary);
        }
        
        .feature-icon {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            color: var(--discord-secondary);
            transition: transform var(--transition-speed);
        }
        
        .feature-card:hover .feature-icon {
            transform: scale(1.2) rotate(10deg);
        }
        
        .feature-title {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--discord-light);
        }
        
        .feature-description {
            color: #B9BBBE;
            line-height: 1.6;
        }
        
        /* Botão do Discord */
        .discord-button-container {
            margin-top: 2rem;
            position: relative;
            perspective: 1000px;
            opacity: 0;
            animation: fade-in 1s forwards 1.5s;
        }
        
        .discord-button {
            display: inline-block;
            padding: 1.2rem 2.5rem;
            font-size: 1.5rem;
            font-weight: 700;
            text-decoration: none;
            color: white;
            background: linear-gradient(45deg, var(--discord-primary), var(--discord-secondary));
            border-radius: 50px;
            box-shadow: 0 5px 20px rgba(88, 101, 242, 0.5);
            transition: all var(--transition-speed);
            position: relative;
            overflow: hidden;
            z-index: 1;
            transform-style: preserve-3d;
            animation: pulse 2s infinite;
        }
        
        .discord-button::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, 
                transparent, 
                rgba(255, 255, 255, 0.3), 
                transparent);
            transform: rotate(45deg);
            z-index: -1;
            animation: shine 3s infinite;
        }
        
        .discord-button:hover {
            transform: scale(1.05) translateY(-5px);
            box-shadow: 0 10px 30px rgba(88, 101, 242, 0.8);
        }
        
        .discord-button:active {
            transform: scale(0.95);
        }
        
        .discord-button i {
            margin-right: 10px;
        }
        
        /* Logo do Discord */
        .discord-logo {
            width: 120px;
            height: 120px;
            margin: 0 auto 2rem;
            background-color: var(--discord-primary);
            mask: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 245 240'%3E%3Cpath d='M104.4 103.9c-5.7 0-10.2 5-10.2 11.1s4.6 11.1 10.2 11.1c5.7 0 10.2-5 10.2-11.1.1-6.1-4.5-11.1-10.2-11.1zm36.5 0c-5.7 0-10.2 5-10.2 11.1s4.6 11.1 10.2 11.1c5.7 0 10.2-5 10.2-11.1s-4.5-11.1-10.2-11.1z'/%3E%3Cpath d='M189.5 20h-134C44.2 20 35 29.2 35 40.6v135.2c0 11.4 9.2 20.6 20.5 20.6h113.4l-5.3-18.5 12.8 11.9 12.1 11.2 21.5 19V40.6c0-11.4-9.2-20.6-20.5-20.6zm-38.6 130.6s-3.6-4.3-6.6-8.1c13.1-3.7 18.1-11.9 18.1-11.9-4.1 2.7-8 4.6-11.5 5.9-5 2.1-9.8 3.5-14.5 4.3-9.6 1.8-18.4 1.3-25.9-.1-5.7-1.1-10.6-2.7-14.7-4.3-2.3-.9-4.8-2-7.3-3.4-.3-.2-.6-.3-.9-.5-.2-.1-.3-.2-.4-.3-1.8-1-2.8-1.7-2.8-1.7s4.8 8 17.5 11.8c-3 3.8-6.7 8.3-6.7 8.3-22.1-.7-30.5-15.2-30.5-15.2 0-32.2 14.4-58.3 14.4-58.3 14.4-10.8 28.1-10.5 28.1-10.5l1 1.2c-18 5.2-26.3 13.1-26.3 13.1s2.2-1.2 5.9-2.9c10.7-4.7 19.2-6 22.7-6.3.6-.1 1.1-.2 1.7-.2 6.1-.8 13-1 20.2-.2 9.5 1.1 19.7 3.9 30.1 9.6 0 0-7.9-7.5-24.9-12.7l1.4-1.6s13.7-.3 28.1 10.5c0 0 14.4 26.1 14.4 58.3 0 0-8.5 14.5-30.6 15.2z'/%3E%3C/svg%3E") no-repeat center;
            -webkit-mask: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 245 240'%3E%3Cpath d='M104.4 103.9c-5.7 0-10.2 5-10.2 11.1s4.6 11.1 10.2 11.1c5.7 0 10.2-5 10.2-11.1.1-6.1-4.5-11.1-10.2-11.1zm36.5 0c-5.7 0-10.2 5-10.2 11.1s4.6 11.1 10.2 11.1c5.7 0 10.2-5 10.2-11.1s-4.5-11.1-10.2-11.1z'/%3E%3Cpath d='M189.5 20h-134C44.2 20 35 29.2 35 40.6v135.2c0 11.4 9.2 20.6 20.5 20.6h113.4l-5.3-18.5 12.8 11.9 12.1 11.2 21.5 19V40.6c0-11.4-9.2-20.6-20.5-20.6zm-38.6 130.6s-3.6-4.3-6.6-8.1c13.1-3.7 18.1-11.9 18.1-11.9-4.1 2.7-8 4.6-11.5 5.9-5 2.1-9.8 3.5-14.5 4.3-9.6 1.8-18.4 1.3-25.9-.1-5.7-1.1-10.6-2.7-14.7-4.3-2.3-.9-4.8-2-7.3-3.4-.3-.2-.6-.3-.9-.5-.2-.1-.3-.2-.4-.3-1.8-1-2.8-1.7-2.8-1.7s4.8 8 17.5 11.8c-3 3.8-6.7 8.3-6.7 8.3-22.1-.7-30.5-15.2-30.5-15.2 0-32.2 14.4-58.3 14.4-58.3 14.4-10.8 28.1-10.5 28.1-10.5l1 1.2c-18 5.2-26.3 13.1-26.3 13.1s2.2-1.2 5.9-2.9c10.7-4.7 19.2-6 22.7-6.3.6-.1 1.1-.2 1.7-.2 6.1-.8 13-1 20.2-.2 9.5 1.1 19.7 3.9 30.1 9.6 0 0-7.9-7.5-24.9-12.7l1.4-1.6s13.7-.3 28.1 10.5c0 0 14.4 26.1 14.4 58.3 0 0-8.5 14.5-30.6 15.2z'/%3E%3C/svg%3E") no-repeat center;
            animation: float 3s ease-in-out infinite, pulse 2s infinite alternate;
            opacity: 0;
            transform: scale(0);
            animation: logo-appear 1s forwards 0.3s;
        }
        
        /* Elementos flutuantes */
        .floating-element {
            position: absolute;
            opacity: 0;
            animation: float-element 10s infinite ease-in-out;
        }
        
        .element-1 {
            top: 10%;
            left: 5%;
            font-size: 3rem;
            color: var(--discord-green);
            animation-delay: 0s;
            animation-duration: 12s;
        }
        
        .element-2 {
            top: 20%;
            right: 10%;
            font-size: 4rem;
            color: var(--discord-yellow);
            animation-delay: 2s;
            animation-duration: 15s;
        }
        
        .element-3 {
            bottom: 15%;
            left: 15%;
            font-size: 3.5rem;
            color: var(--discord-accent);
            animation-delay: 1s;
            animation-duration: 14s;
        }
        
        .element-4 {
            bottom: 25%;
            right: 5%;
            font-size: 2.5rem;
            color: var(--discord-red);
            animation-delay: 3s;
            animation-duration: 13s;
        }
        
        .element-5 {
            top: 50%;
            left: 10%;
            font-size: 3rem;
            color: var(--discord-purple);
            animation-delay: 1.5s;
            animation-duration: 16s;
        }
        
        .element-6 {
            top: 40%;
            right: 15%;
            font-size: 2.8rem;
            color: var(--discord-orange);
            animation-delay: 2.5s;
            animation-duration: 17s;
        }
        
        /* Seção de rodapé */
        .footer {
            margin-top: 3rem;
            text-align: center;
            opacity: 0;
            animation: fade-in 1s forwards 2s;
        }
        
        .footer p {
            color: #B9BBBE;
            margin-bottom: 1rem;
        }
        
        .social-icons {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-top: 1rem;
        }
        
        .social-icon {
            font-size: 1.5rem;
            color: var(--discord-secondary);
            transition: all var(--transition-speed);
        }
        
        .social-icon:hover {
            color: var(--discord-light);
            transform: translateY(-5px);
        }
        
        /* Animações */
        @keyframes fade-in {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        @keyframes fade-in-up {
            from { 
                opacity: 0; 
                transform: translateY(50px);
            }
            to { 
                opacity: 1; 
                transform: translateY(0);
            }
        }
        
        @keyframes letter-bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-15px); }
        }
        
        @keyframes card-appear {
            from { 
                opacity: 0; 
                transform: translateY(50px) rotateX(10deg);
            }
            to { 
                opacity: 1; 
                transform: translateY(0) rotateX(0);
            }
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }
        
        @keyframes shine {
            0% { transform: translateX(-100%) rotate(45deg); }
            100% { transform: translateX(100%) rotate(45deg); }
        }
        
        @keyframes float-element {
            0% { 
                opacity: 0; 
                transform: translateY(0) translateX(0) rotate(0deg); 
            }
            10% { 
                opacity: 1; 
            }
            50% { 
                transform: translateY(-100px) translateX(50px) rotate(10deg); 
            }
            90% { 
                opacity: 1; 
            }
            100% { 
                opacity: 0; 
                transform: translateY(0) translateX(0) rotate(0deg); 
            }
        }
        
        @keyframes float-particle {
            0% { 
                transform: translateY(0) translateX(0); 
            }
            25% { 
                transform: translateY(-100vh) translateX(100vw); 
            }
            50% { 
                transform: translateY(-50vh) translateX(50vw); 
            }
            75% { 
                transform: translateY(-100vh) translateX(0); 
            }
            100% { 
                transform: translateY(0) translateX(0); 
            }
        }
        
        @keyframes logo-appear {
            from { 
                opacity: 0; 
                transform: scale(0) rotate(-180deg);
            }
            to { 
                opacity: 1; 
                transform: scale(1) rotate(0);
            }
        }
        
        /* Efeito de parallax */
        .parallax-layer {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
        }
        
        .layer-1 {
            background: radial-gradient(circle, rgba(88, 101, 242, 0.2) 0%, transparent 70%);
            transform: translateZ(-10px);
        }
        
        .layer-2 {
            background: radial-gradient(circle, rgba(235, 69, 158, 0.1) 0%, transparent 60%);
            transform: translateZ(-20px);
        }
        
        /* Responsividade */
        @media (max-width: 768px) {
            .welcome-title {
                font-size: 2.5rem;
            }
            
            .welcome-subtitle {
                font-size: 1.2rem;
            }
            
            .features-container {
                flex-direction: column;
                align-items: center;
            }
            
            .feature-card {
                width: 100%;
                max-width: 350px;
            }
            
            .discord-button {
                font-size: 1.2rem;
                padding: 1rem 2rem;
            }
            
            .discord-logo {
                width: 80px;
                height: 80px;
            }
            
            .floating-element {
                font-size: 2rem !important;
            }
        }
    </style>
</head>
<body>
    <!-- Efeito de partículas -->
    <div class="particles-container" id="particles-container"></div>
    
    <!-- Camadas de parallax -->
    <div class="parallax-layer layer-1"></div>
    <div class="parallax-layer layer-2"></div>
    
    <!-- Elementos flutuantes -->
    <div class="floating-element element-1"><i class="fas fa-gamepad"></i></div>
    <div class="floating-element element-2"><i class="fas fa-headset"></i></div>
    <div class="floating-element element-3"><i class="fas fa-comment-alt"></i></div>
    <div class="floating-element element-4"><i class="fas fa-music"></i></div>
    <div class="floating-element element-5"><i class="fas fa-video"></i></div>
    <div class="floating-element element-6"><i class="fas fa-users"></i></div>
    
    <div class="main-container">
        <div class="welcome-section">
            <div class="discord-logo"></div>
            <h1 class="welcome-title">
                <span style="--i:1;">E</span>
                <span style="--i:2;">N</span>
                <span style="--i:3;">T</span>
                <span style="--i:4;">R</span>
                <span style="--i:5;">E</span>
                <span style="--i:6;">&nbsp;</span>
                <span style="--i:7;">N</span>
                <span style="--i:8;">O</span>
                <span style="--i:9;">&nbsp;</span>
                <span style="--i:10;">D</span>
                <span style="--i:11;">I</span>
                <span style="--i:12;">S</span>
                <span style="--i:13;">C</span>
                <span style="--i:14;">O</span>
                <span style="--i:15;">R</span>
                <span style="--i:16;">D</span>
            </h1>
            <p class="welcome-subtitle">A melhor plataforma para se conectar com amigos e comunidades!</p>
        </div>
        
        <div class="features-container">
            <div class="feature-card" style="--card-i:1;">
                <div class="feature-icon"><i class="fas fa-comments"></i></div>
                <h3 class="feature-title">Chat em Tempo Real</h3>
                <p class="feature-description">Converse com seus amigos através de texto, voz e vídeo de forma rápida e segura.</p>
            </div>
            
            <div class="feature-card" style="--card-i:2;">
                <div class="feature-icon"><i class="fas fa-users"></i></div>
                <h3 class="feature-title">Comunidades</h3>
                <p class="feature-description">Participe de servidores temáticos e encontre pessoas com interesses similares.</p>
            </div>
            
            <div class="feature-card" style="--card-i:3;">
                <div class="feature-icon"><i class="fas fa-gamepad"></i></div>
                <h3 class="feature-title">Jogos e Diversão</h3>
                <p class="feature-description">Jogue com amigos, compartilhe tela e divirta-se com atividades em grupo.</p>
            </div>
        </div>
        
        <div class="discord-button-container">
            <a href="https://discord.gg/g9VYhbSa6x" class="discord-button" target="_blank">
                <i class="fab fa-discord"></i> ENTRAR AGORA
            </a>
        </div>
        
        <div class="footer">
            <p>Junte-se a milhões de pessoas que já estão no Discord!</p>
            <div class="social-icons">
                <a href="#" class="social-icon"><i class="fab fa-twitter"></i></a>
                <a href="#" class="social-icon"><i class="fab fa-instagram"></i></a>
                <a href="#" class="social-icon"><i class="fab fa-facebook"></i></a>
                <a href="#" class="social-icon"><i class="fab fa-youtube"></i></a>
            </div>
        </div>
    </div>
    
    <script>
        // Criar partículas
        document.addEventListener('DOMContentLoaded', function() {
            const particlesContainer = document.getElementById('particles-container');
            const colors = [
                '#5865F2', '#57F287', '#FEE75C', '#EB459E', '#ED4245', 
                '#FFFFFF', '#9B59B6', '#E67E22'
            ];
            
            // Criar 50 partículas
            for (let i = 0; i < 50; i++) {
                createParticle();
            }
            
            function createParticle() {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                
                // Tamanho aleatório
                const size = Math.random() * 10 + 5;
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                
                // Posição aleatória
                particle.style.top = `${Math.random() * 100}%`;
                particle.style.left = `${Math.random() * 100}%`;
                
                // Cor aleatória
                const color = colors[Math.floor(Math.random() * colors.length)];
                particle.style.backgroundColor = color;
                
                // Duração da animação aleatória
                const duration = Math.random() * 20 + 10;
                particle.style.animationDuration = `${duration}s`;
                
                // Atraso da animação aleatório
                const delay = Math.random() * 10;
                particle.style.animationDelay = `${delay}s`;
                
                particlesContainer.appendChild(particle);
            }
            
            // Efeito de parallax
            document.addEventListener('mousemove', function(e) {
                const xAxis = (window.innerWidth / 2 - e.pageX) / 25;
                const yAxis = (window.innerHeight / 2 - e.pageY) / 25;
                
                const elements = document.querySelectorAll('.floating-element');
                elements.forEach(element => {
                    const speed = parseFloat(element.getAttribute('data-speed') || 1);
                    element.style.transform = `translate(${xAxis * speed}px, ${yAxis * speed}px)`;
                });
            });
            
            // Animação de entrada dos elementos
            const featureCards = document.querySelectorAll('.feature-card');
            featureCards.forEach((card, index) => {
                card.style.animationDelay = `${0.3 + (index * 0.2)}s`;
            });
            
            // Efeito de hover nos cards
            featureCards.forEach(card => {
                card.addEventListener('mouseenter', function() {
                    this.style.transform = 'translateY(-10px) rotateX(0deg)';
                    this.style.boxShadow = '0 15px 40px rgba(88, 101, 242, 0.4)';
                    this.style.borderColor = 'var(--discord-secondary)';
                });
                
                card.addEventListener('mouseleave', function() {
                    this.style.transform = '';
                    this.style.boxShadow = '';
                    this.style.borderColor = '';
                });
            });
            
            // Efeito de clique no botão
            const discordButton = document.querySelector('.discord-button');
            discordButton.addEventListener('mousedown', function() {
                this.style.transform = 'scale(0.95)';
            });
            
            discordButton.addEventListener('mouseup', function() {
                this.style.transform = 'scale(1.05) translateY(-5px)';
            });
            
            // Animação de entrada
            document.querySelector('.main-container').style.opacity = '0';
            document.querySelector('.main-container').style.transform = 'translateY(50px)';
            document.querySelector('.main-container').style.transition = 'opacity 1s ease, transform 1s ease';
            
            setTimeout(() => {
                document.querySelector('.main-container').style.opacity = '1';
                document.querySelector('.main-container').style.transform = 'translateY(0)';
            }, 300);
        });
    </script>
</body>
</html>
