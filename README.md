<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dhruvil Patel - GitHub Profile</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 20px;
            background: linear-gradient(135deg, #0f0f0f 0%, #1a1a1a 100%);
            color: #ffffff;
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
        }
        .container {
            max-width: 900px;
            margin: 0 auto;
        }
        .hero-section {
            background: linear-gradient(135deg, #1a1a1a 0%, #2a2a2a 50%, #1a1a1a 100%);
            padding: 60px 40px;
            border-radius: 20px;
            text-align: center;
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
            box-shadow: 0 20px 40px rgba(0,0,0,0.3);
        }
        .hero-section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 3px;
            background: linear-gradient(90deg, #FF6B6B, #4ECDC4, #45B7D1, #96CEB4, #FFEAA7);
            animation: shimmer 3s linear infinite;
        }
        @keyframes shimmer {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }
        .hero-title {
            font-size: 3.5rem;
            font-weight: 700;
            background: linear-gradient(135deg, #FF6B6B, #4ECDC4);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 10px;
        }
        .hero-subtitle {
            font-size: 1.3rem;
            color: #B0B0B0;
            margin-bottom: 30px;
        }
        .section {
            background: rgba(42, 42, 42, 0.8);
            backdrop-filter: blur(10px);
            padding: 30px;
            border-radius: 15px;
            margin-bottom: 25px;
            box-shadow: 0 8px 32px rgba(0,0,0,0.2);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0,0,0,0.3);
        }
        .section-title {
            font-size: 1.8rem;
            font-weight: 600;
            color: #4ECDC4;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }
        .tech-item {
            background: rgba(255, 255, 255, 0.05);
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        .tech-item:hover {
            background: rgba(255, 255, 255, 0.1);
            transform: translateY(-3px);
        }
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        .stat-item {
            text-align: center;
        }
        .stat-item img {
            max-width: 100%;
            border-radius: 10px;
            transition: transform 0.3s ease;
        }
        .stat-item img:hover {
            transform: scale(1.05);
        }
        .contact-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin-top: 20px;
        }
        .contact-link {
            background: linear-gradient(135deg, #FF6B6B, #4ECDC4);
            color: white;
            text-decoration: none;
            padding: 12px 24px;
            border-radius: 25px;
            font-weight: 500;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }
        .contact-link:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(255, 107, 107, 0.3);
        }
        .skills-category {
            margin-bottom: 25px;
        }
        .skills-category h4 {
            color: #FF6B6B;
            margin-bottom: 15px;
            font-size: 1.1rem;
            font-weight: 600;
        }
        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        .skill-tag {
            background: rgba(78, 205, 196, 0.2);
            color: #4ECDC4;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9rem;
            border: 1px solid rgba(78, 205, 196, 0.3);
            transition: all 0.3s ease;
        }
        .skill-tag:hover {
            background: rgba(78, 205, 196, 0.3);
            transform: scale(1.05);
        }
        .animated-text {
            background: linear-gradient(-45deg, #FF6B6B, #4ECDC4, #45B7D1, #96CEB4);
            background-size: 400% 400%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: gradientShift 4s ease-in-out infinite;
        }
        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }
        .github-calendar {
            margin-top: 20px;
        }
        .footer {
            text-align: center;
            margin: 50px 0;
            padding: 30px;
            background: rgba(42, 42, 42, 0.5);
            border-radius: 15px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        @media (max-width: 768px) {
            .hero-title { font-size: 2.5rem; }
            .tech-grid { grid-template-columns: repeat(auto-fit, minmax(100px, 1fr)); }
            .stats-container { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Hero Section -->
        <div class="hero-section">
            <h1 class="hero-title">👋 Hi, I'm Dhruvil Patel</h1>
            <p class="hero-subtitle">@Dhruvilpatel2303</p>
            <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&duration=3000&pause=1000&color=4ECDC4&center=true&vCenter=true&width=600&lines=Full+Stack+Developer+%F0%9F%9A%80;Android+%26+Backend+Specialist+%F0%9F%93%B1;Microservices+Architect+%E2%9A%A1;Cloud+%26+DevOps+Enthusiast+%E2%98%81%EF%B8%8F;Always+Learning%2C+Always+Building+%F0%9F%9B%A0%EF%B8%8F" alt="Typing animation" style="margin: 20px 0;">
            <div class="contact-links">
                <a href="mailto:pateldhruvil2303@gmail.com" class="contact-link">📧 Email</a>
                <a href="https://www.linkedin.com/in/dhruvil-patel-507301285/" class="contact-link">💼 LinkedIn</a>
                <a href="https://github.com/Dhruvilpatel2303" class="contact-link">🐙 GitHub</a>
            </div>
        </div>

        <!-- About Section -->
        <div class="section">
            <h2 class="section-title">🚀 About Me</h2>
            <p style="font-size: 1.1rem; color: #D0D0D0;">
                I'm a passionate <span class="animated-text"><strong>Full Stack Developer</strong></span> with expertise in building scalable mobile applications and robust backend systems. I specialize in <strong style="color: #4ECDC4;">Android development</strong> with modern technologies like <strong style="color: #4ECDC4;">Jetpack Compose</strong>, and backend development using <strong style="color: #4ECDC4;">Spring Boot microservices</strong>, <strong style="color: #4ECDC4;">Apache Kafka</strong>, and cloud technologies.
            </p>
            <p style="font-size: 1.1rem; color: #D0D0D0; margin-top: 15px;">
                I'm passionate about creating efficient, scalable solutions and staying up-to-date with the latest technology trends. I enjoy working on challenging projects that involve real-time data processing, distributed systems, and seamless user experiences.
            </p>
        </div>

        <!-- Technical Skills -->
        <div class="section">
            <h2 class="section-title">🛠️ Technical Skills</h2>
            
            <div class="skills-category">
                <h4>📱 Mobile Development</h4>
                <div class="skill-tags">
                    <span class="skill-tag">Android</span>
                    <span class="skill-tag">Kotlin</span>
                    <span class="skill-tag">Jetpack Compose</span>
                    <span class="skill-tag">MVVM</span>
                    <span class="skill-tag">Clean Architecture</span>
                    <span class="skill-tag">Retrofit</span>
                    <span class="skill-tag">Room Database</span>
                    <span class="skill-tag">Coroutines</span>
                </div>
            </div>

            <div class="skills-category">
                <h4>⚙️ Backend Development</h4>
                <div class="skill-tags">
                    <span class="skill-tag">Spring Boot</span>
                    <span class="skill-tag">Spring Security</span>
                    <span class="skill-tag">Spring Data JPA</span>
                    <span class="skill-tag">Microservices</span>
                    <span class="skill-tag">Ktor</span>
                    <span class="skill-tag">Flask</span>
                    <span class="skill-tag">REST APIs</span>
                    <span class="skill-tag">GraphQL</span>
                </div>
            </div>

            <div class="skills-category">
                <h4>🗃️ Databases</h4>
                <div class="skill-tags">
                    <span class="skill-tag">MongoDB</span>
                    <span class="skill-tag">PostgreSQL</span>
                    <span class="skill-tag">MySQL</span>
                    <span class="skill-tag">Redis</span>
                    <span class="skill-tag">Firebase Firestore</span>
                    <span class="skill-tag">Supabase</span>
                </div>
            </div>

            <div class="skills-category">
                <h4>🔄 Message Queues & Streaming</h4>
                <div class="skill-tags">
                    <span class="skill-tag">Apache Kafka</span>
                    <span class="skill-tag">RabbitMQ</span>
                    <span class="skill-tag">WebSockets</span>
                    <span class="skill-tag">Server-Sent Events</span>
                </div>
            </div>

            <div class="skills-category">
                <h4>☁️ Cloud & DevOps</h4>
                <div class="skill-tags">
                    <span class="skill-tag">Docker</span>
                    <span class="skill-tag">Kubernetes</span>
                    <span class="skill-tag">AWS</span>
                    <span class="skill-tag">Google Cloud</span>
                    <span class="skill-tag">CI/CD</span>
                    <span class="skill-tag">GitHub Actions</span>
                    <span class="skill-tag">Jenkins</span>
                </div>
            </div>

            <div class="skills-category">
                <h4>🧪 Testing & Tools</h4>
                <div class="skill-tags">
                    <span class="skill-tag">JUnit</span>
                    <span class="skill-tag">Mockito</span>
                    <span class="skill-tag">Espresso</span>
                    <span class="skill-tag">Postman</span>
                    <span class="skill-tag">Git</span>
                    <span class="skill-tag">Maven</span>
                    <span class="skill-tag">Gradle</span>
                </div>
            </div>
        </div>

        <!-- Current Focus -->
        <div class="section">
            <h2 class="section-title">🌱 Currently Learning & Building</h2>
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;">
                <div style="background: rgba(255, 107, 107, 0.1); padding: 20px; border-radius: 10px; border: 1px solid rgba(255, 107, 107, 0.2);">
                    <h4 style="color: #FF6B6B; margin-bottom: 10px;">🏗️ Architecture & Design</h4>
                    <ul style="color: #D0D0D0; margin: 0; padding-left: 20px;">
                        <li>Event-driven microservices architecture</li>
                        <li>Domain-driven design patterns</li>
                        <li>CQRS and Event Sourcing</li>
                    </ul>
                </div>
                <div style="background: rgba(78, 205, 196, 0.1); padding: 20px; border-radius: 10px; border: 1px solid rgba(78, 205, 196, 0.2);">
                    <h4 style="color: #4ECDC4; margin-bottom: 10px;">🤖 AI/ML Integration</h4>
                    <ul style="color: #D0D0D0; margin: 0; padding-left: 20px;">
                        <li>TensorFlow Lite for Android</li>
                        <li>ML model deployment strategies</li>
                        <li>Real-time inference pipelines</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Technologies -->
        <div class="section">
            <h2 class="section-title">💻 Tech Stack</h2>
            <div class="tech-grid">
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white" alt="Kafka" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white" alt="RabbitMQ" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" alt="AWS" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/Jetpack_Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white" alt="Jetpack Compose" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" alt="Firebase" style="width: 100%; max-width: 150px;">
                </div>
                <div class="tech-item">
                    <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" style="width: 100%; max-width: 150px;">
                </div>
            </div>
        </div>

        <!-- Collaboration -->
        <div class="section">
            <h2 class="section-title">🤝 Open to Collaborate On</h2>
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin-top: 20px;">
                <div style="background: rgba(255, 255, 255, 0.05); padding: 20px; border-radius: 10px;">
                    <h4 style="color: #FF6B6B; margin-bottom: 10px;">📱 Mobile Projects</h4>
                    <p style="color: #D0D0D0; font-size: 0.95rem;">Android apps with modern architecture, real-time features, and cloud integration</p>
                </div>
                <div style="background: rgba(255, 255, 255, 0.05); padding: 20px; border-radius: 10px;">
                    <h4 style="color: #4ECDC4; margin-bottom: 10px;">🏗️ Backend Systems</h4>
                    <p style="color: #D0D0D0; font-size: 0.95rem;">Microservices, event-driven architectures, and distributed systems</p>
                </div>
                <div style="background: rgba(255, 255, 255, 0.05); padding: 20px; border-radius: 10px;">
                    <h4 style="color: #45B7D1; margin-bottom: 10px;">🌐 Full Stack</h4>
                    <p style="color: #D0D0D0; font-size: 0.95rem;">End-to-end applications with modern tech stack and best practices</p>
                </div>
                <div style="background: rgba(255, 255, 255, 0.05); padding: 20px; border-radius: 10px;">
                    <h4 style="color: #96CEB4; margin-bottom: 10px;">🔓 Open Source</h4>
                    <p style="color: #D0D0D0; font-size: 0.95rem;">Libraries, tools, and community-driven projects</p>
                </div>
            </div>
        </div>

        <!-- GitHub Stats -->
        <div class="section">
            <h2 class="section-title">📈 GitHub Analytics</h2>
            <div class="stats-container">
                <div class="stat-item">
                    <img src="https://github-readme-stats.vercel.app/api?username=Dhruvilpatel2303&show_icons=true&theme=tokyonight&hide_border=true&bg_color=1a1a1a&title_color=4ECDC4&icon_color=FF6B6B&text_color=ffffff" alt="GitHub Stats">
                </div>
                <div class="stat-item">
                    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Dhruvilpatel2303&layout=donut&theme=tokyonight&hide_border=true&bg_color=1a1a1a&title_color=4ECDC4&text_color=ffffff" alt="Top Languages">
                </div>
            </div>
            <div style="text-align: center; margin-top: 20px;">
                <img src="https://github-readme-streak-stats.herokuapp.com/?user=Dhruvilpatel2303&theme=tokyonight&hide_border=true&background=1a1a1a&stroke=4ECDC4&ring=FF6B6B&fire=FF6B6B&currStreakLabel=4ECDC4" alt="GitHub Streak" style="max-width: 100%;">
            </div>
            <div class="github-calendar" style="text-align: center;">
                <img src="https://github-readme-activity-graph.vercel.app/graph?username=Dhruvilpatel2303&bg_color=1a1a1a&color=4ECDC4&line=FF6B6B&point=ffffff&area=true&hide_border=true" alt="Activity Graph" style="max-width: 100%; border-radius: 10px;">
            </div>
        </div>

        <!-- Trophies -->
        <div class="section">
            <h2 class="section-title">🏆 GitHub Trophies</h2>
            <div style="text-align: center;">
                <img src="https://github-profile-trophy.vercel.app/?username=Dhruvilpatel2303&theme=tokyonight&no-frame=true&no-bg=true&margin-w=4&column=4" alt="GitHub Trophies" style="max-width: 100%;">
            </div>
        </div>

        <!-- Footer -->
        <div class="footer">
            <h3 class="animated-text">🚀 Always learning. Always building. Always improving.</h3>
            <p style="color: #B0B0B0; font-size: 1.1rem; margin-top: 20px;">
                Let's connect and create something amazing together! 🌟
            </p>
            <div style="margin-top: 20px;">
                <img src="https://komarev.com/ghpvc/?username=Dhruvilpatel2303&label=Profile%20views&color=4ECDC4&style=flat-square" alt="Profile Views">
            </div>
        </div>
    </div>

    <script>
        // Add smooth scrolling and interactive elements
        document.addEventListener('DOMContentLoaded', function() {
            // Add hover effects to sections
            const sections = document.querySelectorAll('.section');
            sections.forEach(section => {
                section.addEventListener('mouseenter', function() {
                    this.style.transform = 'translateY(-8px)';
                    this.style.boxShadow = '0 20px 50px rgba(0,0,0,0.4)';
                });
                
                section.addEventListener('mouseleave', function() {
                    this.style.transform = 'translateY(0)';
                    this.style.boxShadow = '0 8px 32px rgba(0,0,0,0.2)';
                });
            });

            // Add click animation to contact links
            const contactLinks = document.querySelectorAll('.contact-link');
            contactLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    this.style.transform = 'scale(0.95)';
                    setTimeout(() => {
                        this.style.transform = 'scale(1)';
                    }, 150);
                });
            });

            // Add floating animation to skill tags
            const skillTags = document.querySelectorAll('.skill-tag');
            skillTags.forEach((tag, index) => {
                tag.style.animationDelay = `${index * 0.1}s`;
                tag.addEventListener('mouseenter', function() {
                    this.style.transform = 'scale(1.1) rotate(2deg)';
                });
                tag.addEventListener('mouseleave', function() {
                    this.style.transform = 'scale(1) rotate(0deg)';
                });
            });
        });
    </script>
</body>
</html>
