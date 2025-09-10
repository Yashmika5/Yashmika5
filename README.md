<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gajindu Yashmika - Full Stack Developer</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Roboto+Mono:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
            color: #f0f6fc;
            line-height: 1.6;
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header & Hero Section */
        .hero {
            text-align: center;
            padding: 80px 0 40px;
            position: relative;
            overflow: hidden;
        }

        .hero-bg {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            opacity: 0.1;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" width="100" height="100" fill="%23FFFFFF"><circle cx="50" cy="50" r="2"/></svg>');
            z-index: -1;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 16px;
            font-weight: 700;
            background: linear-gradient(90deg, #64ffda, #00a2ff, #ff00cc);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            animation: gradientMove 5s ease infinite;
            background-size: 300% 300%;
        }

        @keyframes gradientMove {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .hero h3 {
            font-size: 1.8rem;
            margin-bottom: 24px;
            font-weight: 500;
            color: #c9d1d9;
            opacity: 0;
            animation: fadeIn 1s ease forwards;
            animation-delay: 0.5s;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .profile-views {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            display: inline-block;
            padding: 8px 16px;
            border-radius: 30px;
            margin: 20px 0;
            font-size: 0.9rem;
            border: 1px solid rgba(255, 255, 255, 0.2);
            opacity: 0;
            animation: fadeIn 1s ease forwards;
            animation-delay: 1s;
        }

        /* About Section */
        .about {
            padding: 40px 0;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }

        .about p {
            margin-bottom: 20px;
            font-size: 1.1rem;
            color: #c9d1d9;
            opacity: 0;
            animation: fadeIn 1s ease forwards;
            animation-delay: 0.8s;
        }

        .email-link {
            display: inline-block;
            background: linear-gradient(90deg, #ff6b6b, #ff8e53);
            color: white;
            padding: 12px 24px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 500;
            margin-top: 10px;
            transition: all 0.3s ease;
            opacity: 0;
            animation: fadeIn 1s ease forwards;
            animation-delay: 1.2s;
            box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
        }

        .email-link:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(255, 107, 107, 0.4);
        }

        /* Social Links */
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 40px 0;
            flex-wrap: wrap;
        }

        .social-link {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(255, 255, 255, 0.1);
            color: white;
            font-size: 1.5rem;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.2);
            opacity: 0;
            animation: fadeIn 1s ease forwards;
            animation-delay: calc(0.2s * var(--i));
        }

        .social-link:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateY(-5px) scale(1.1);
        }

        /* Skills Section */
        .skills {
            padding: 60px 0;
        }

        .section-title {
            text-align: center;
            font-size: 2.2rem;
            margin-bottom: 40px;
            color: #64ffda;
            position: relative;
            display: inline-block;
            left: 50%;
            transform: translateX(-50%);
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 100%;
            height: 3px;
            background: linear-gradient(90deg, #64ffda, transparent);
            border-radius: 3px;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(80px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .skill-item {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            padding: 15px;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0;
            animation: fadeIn 0.5s ease forwards;
            animation-delay: calc(0.05s * var(--i));
        }

        .skill-item:hover {
            transform: translateY(-5px);
            background: rgba(255, 255, 255, 0.1);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .skill-icon {
            font-size: 2rem;
            margin-bottom: 10px;
            color: #64ffda;
        }

        .skill-name {
            font-size: 0.8rem;
            color: #c9d1d9;
        }

        /* Stats Section */
        .stats {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin: 60px 0;
            flex-wrap: wrap;
        }

        .stat-item {
            text-align: center;
            background: rgba(255, 255, 255, 0.05);
            padding: 20px;
            border-radius: 10px;
            min-width: 200px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0;
            animation: fadeIn 1s ease forwards;
            animation-delay: 0.5s;
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            background: linear-gradient(90deg, #64ffda, #00a2ff);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .stat-label {
            font-size: 1rem;
            color: #8b949e;
            margin-top: 5px;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero h3 {
                font-size: 1.4rem;
            }
            
            .skills-grid {
                grid-template-columns: repeat(auto-fill, minmax(70px, 1fr));
            }
            
            .stats {
                gap: 15px;
            }
            
            .stat-item {
                min-width: 150px;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .social-link {
                width: 50px;
                height: 50px;
                font-size: 1.2rem;
            }
            
            .stats {
                flex-direction: column;
                align-items: center;
            }
            
            .stat-item {
                width: 100%;
                max-width: 250px;
            }
        }

        /* Particle Animation */
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }

        .particle {
            position: absolute;
            border-radius: 50%;
            background: rgba(100, 255, 218, 0.3);
            animation: float 15s infinite linear;
        }

        @keyframes float {
            0% {
                transform: translateY(0) translateX(0) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(-100vh) translateX(100vw) rotate(360deg);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <div class="particles" id="particles"></div>
    
    <div class="container">
        <section class="hero">
            <div class="hero-bg"></div>
            <h1 class="animated-title">Hi 👋, I'm Gajindu Yashmika</h1>
            <h3>A passionate Full Stack Developer from Sri Lanka</h3>
            
            <div class="profile-views">
                <i class="fas fa-eye"></i> <span id="view-count">0</span> Profile Views
            </div>
        </section>

        <section class="about">
            <p>I'm a passionate full stack developer with experience in building web and mobile applications using modern technologies. I enjoy turning complex problems into simple, beautiful and intuitive solutions.</p>
            <a href="mailto:gajinduyashmika5@gmail.com" class="email-link">
                <i class="fas fa-envelope"></i> Contact Me
            </a>
        </section>

        <div class="social-links">
            <a href="https://twitter.com/3" target="_blank" class="social-link" style="--i: 1;">
                <i class="fab fa-twitter"></i>
            </a>
            <a href="https://linkedin.com/in/yashmika5" target="_blank" class="social-link" style="--i: 2;">
                <i class="fab fa-linkedin-in"></i>
            </a>
            <a href="https://kaggle.com/gajinduyashmika" target="_blank" class="social-link" style="--i: 3;">
                <i class="fab fa-kaggle"></i>
            </a>
            <a href="https://fb.com/100081347803846" target="_blank" class="social-link" style="--i: 4;">
                <i class="fab fa-facebook-f"></i>
            </a>
            <a href="https://instagram.com/yashmika_5" target="_blank" class="social-link" style="--i: 5;">
                <i class="fab fa-instagram"></i>
            </a>
        </div>

        <section class="skills">
            <h2 class="section-title">Languages & Tools</h2>
            <div class="skills-grid">
                <!-- Each skill item has a delay based on index -->
                <div class="skill-item" style="--i: 0;">
                    <div class="skill-icon"><i class="fab fa-android"></i></div>
                    <div class="skill-name">Android</div>
                </div>
                <div class="skill-item" style="--i: 1;">
                    <div class="skill-icon"><i class="fab fa-angular"></i></div>
                    <div class="skill-name">Angular</div>
                </div>
                <div class="skill-item" style="--i: 2;">
                    <div class="skill-icon"><i class="fas fa-microchip"></i></div>
                    <div class="skill-name">Arduino</div>
                </div>
                <div class="skill-item" style="--i: 3;">
                    <div class="skill-icon"><i class="fab fa-bootstrap"></i></div>
                    <div class="skill-name">Bootstrap</div>
                </div>
                <div class="skill-item" style="--i: 4;">
                    <div class="skill-icon"><i class="fab fa-cuttlefish"></i></div>
                    <div class="skill-name">C</div>
                </div>
                <div class="skill-item" style="--i: 5;">
                    <div class="skill-icon"><i class="fab fa-cplusplus"></i></div>
                    <div class="skill-name">C++</div>
                </div>
                <div class="skill-item" style="--i: 6;">
                    <div class="skill-icon"><i class="fab fa-microsoft"></i></div>
                    <div class="skill-name">C#</div>
                </div>
                <div class="skill-item" style="--i: 7;">
                    <div class="skill-icon"><i class="fab fa-css3-alt"></i></div>
                    <div class="skill-name">CSS3</div>
                </div>
                <div class="skill-item" style="--i: 8;">
                    <div class="skill-icon"><i class="fab fa-dart"></i></div>
                    <div class="skill-name">Dart</div>
                </div>
                <div class="skill-item" style="--i: 9;">
                    <div class="skill-icon"><i class="fab fa-react"></i></div>
                    <div class="skill-name">React</div>
                </div>
                <!-- Additional skills would continue here -->
            </div>
        </section>

        <div class="stats">
            <div class="stat-item">
                <div class="stat-number">20+</div>
                <div class="stat-label">Projects</div>
            </div>
            <div class="stat-item">
                <div class="stat-number">15+</div>
                <div class="stat-label">Technologies</div>
            </div>
            <div class="stat-item">
                <div class="stat-number" id="github-views">0</div>
                <div class="stat-label">Profile Views</div>
            </div>
        </div>
    </div>

    <script>
        // Animated counter for profile views
        function animateValue(element, start, end, duration) {
            let startTimestamp = null;
            const step = (timestamp) => {
                if (!startTimestamp) startTimestamp = timestamp;
                const progress = Math.min((timestamp - startTimestamp) / duration, 1);
                const value = Math.floor(progress * (end - start) + start);
                element.textContent = value.toLocaleString();
                if (progress < 1) {
                    window.requestAnimationFrame(step);
                }
            };
            window.requestAnimationFrame(step);
        }

        // Initialize counters with example values
        document.addEventListener('DOMContentLoaded', function() {
            const viewCount = document.getElementById('view-count');
            const githubViews = document.getElementById('github-views');
            
            // Simulate view counts - in a real scenario, you would fetch these from an API
            animateValue(viewCount, 0, 1284, 2000);
            animateValue(githubViews, 0, 1284, 2000);
            
            createParticles();
        });

        // Create background particles
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 30;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                
                // Random properties
                const size = Math.random() * 10 + 2;
                const posX = Math.random() * 100;
                const posY = Math.random() * 100;
                const delay = Math.random() * 15;
                const duration = Math.random() * 10 + 15;
                
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                particle.style.left = `${posX}vw`;
                particle.style.top = `${posY}vh`;
                particle.style.animationDelay = `${delay}s`;
                particle.style.animationDuration = `${duration}s`;
                
                particlesContainer.appendChild(particle);
            }
        }
    </script>
</body>
</html>
