![logo](https://github.com/zeeshan2266/zeeshan2266/blob/main/github-header-image%20(2).png)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zeeshan Ahmad - Frontend Developer</title>
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
            background: linear-gradient(135deg, #0f172a, #1e293b);
            color: #e2e8f0;
            line-height: 1.6;
            padding: 2rem;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        header {
            text-align: center;
            margin-bottom: 3rem;
            padding-top: 1rem;
        }
        
        h1 {
            font-size: 3.5rem;
            background: linear-gradient(90deg, #818cf8, #60a5fa, #38bdf8);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 0.5rem;
            font-weight: 700;
            letter-spacing: -0.5px;
        }
        
        .tagline {
            font-size: 1.5rem;
            color: #94a3b8;
            margin-bottom: 1.5rem;
            position: relative;
            display: inline-block;
        }
        
        .tagline::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(90deg, #818cf8, #38bdf8);
            border-radius: 2px;
        }
        
        .banner {
            display: flex;
            justify-content: center;
            margin: 2rem 0;
        }
        
        .banner img {
            max-width: 100%;
            border-radius: 16px;
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.5);
            border: 2px solid #334155;
        }
        
        .content-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
            margin-bottom: 3rem;
        }
        
        @media (max-width: 768px) {
            .content-grid {
                grid-template-columns: 1fr;
            }
        }
        
        .card {
            background: rgba(30, 41, 59, 0.7);
            backdrop-filter: blur(10px);
            border-radius: 16px;
            padding: 2rem;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.3);
            border: 1px solid #334155;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.5);
        }
        
        .card h2 {
            font-size: 1.8rem;
            color: #60a5fa;
            margin-bottom: 1.5rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .card h2 i {
            color: #818cf8;
        }
        
        .section-title {
            font-size: 2.5rem;
            text-align: center;
            margin: 3rem 0 2rem;
            color: #e2e8f0;
            position: relative;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: linear-gradient(90deg, #818cf8, #38bdf8);
            border-radius: 2px;
        }
        
        .focus-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-bottom: 3rem;
        }
        
        .focus-item {
            background: rgba(30, 41, 59, 0.7);
            border-radius: 12px;
            padding: 1.5rem;
            display: flex;
            flex-direction: column;
            border: 1px solid #334155;
        }
        
        .focus-item i {
            font-size: 2rem;
            color: #60a5fa;
            margin-bottom: 1rem;
        }
        
        .focus-item h3 {
            font-size: 1.4rem;
            margin-bottom: 0.8rem;
            color: #e2e8f0;
        }
        
        .progress-container {
            margin: 1.5rem 0;
        }
        
        .progress-title {
            display: flex;
            justify-content: space-between;
            margin-bottom: 0.5rem;
            font-weight: 500;
        }
        
        .progress-bar {
            height: 12px;
            background: #334155;
            border-radius: 10px;
            overflow: hidden;
        }
        
        .progress-fill {
            height: 100%;
            border-radius: 10px;
            position: relative;
        }
        
        .progress-fill::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-image: linear-gradient(90deg, 
                rgba(129, 140, 248, 0.8), 
                rgba(96, 165, 250, 0.8));
            animation: shimmer 2s infinite linear;
            background-size: 200% 100%;
        }
        
        @keyframes shimmer {
            0% { background-position: 100% 0; }
            100% { background-position: -100% 0; }
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
            gap: 1.5rem;
            margin-top: 1.5rem;
        }
        
        .skill-item {
            background: rgba(30, 41, 59, 0.7);
            border-radius: 12px;
            padding: 1.2rem 1rem;
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
            border: 1px solid #334155;
            transition: all 0.3s ease;
        }
        
        .skill-item:hover {
            transform: translateY(-5px);
            background: rgba(56, 70, 100, 0.7);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.3);
        }
        
        .skill-item i {
            font-size: 2rem;
            color: #60a5fa;
        }
        
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }
        
        .contact-item {
            background: rgba(30, 41, 59, 0.7);
            border-radius: 12px;
            padding: 1.5rem;
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
            border: 1px solid #334155;
            transition: all 0.3s ease;
        }
        
        .contact-item:hover {
            transform: translateY(-5px);
            background: rgba(56, 70, 100, 0.7);
        }
        
        .contact-item a {
            color: #60a5fa;
            text-decoration: none;
            font-weight: 500;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .contact-item a:hover {
            color: #38bdf8;
            text-decoration: underline;
        }
        
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin: 3rem 0;
        }
        
        .stat-card {
            background: rgba(30, 41, 59, 0.7);
            border-radius: 16px;
            padding: 1.5rem;
            text-align: center;
            border: 1px solid #334155;
        }
        
        .stat-card h3 {
            font-size: 1.5rem;
            color: #94a3b8;
            margin-bottom: 1rem;
        }
        
        .stat-value {
            font-size: 2.5rem;
            font-weight: 700;
            color: #60a5fa;
            margin-bottom: 1rem;
        }
        
        footer {
            text-align: center;
            padding: 2rem 0;
            color: #94a3b8;
            font-size: 1rem;
            margin-top: 2rem;
            border-top: 1px solid #334155;
        }
        
        .highlight {
            color: #60a5fa;
            font-weight: 500;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Zeeshan Ahmad</h1>
            <div class="tagline">Frontend Developer & UI/UX Enthusiast</div>
            
            <div class="banner">
                <img src="https://i.pinimg.com/originals/54/e3/7d/54e37d8074ebcde1d96c77d7b2a7f310.gif" alt="Coding Animation">
            </div>
        </header>
        
        <div class="content-grid">
            <div class="card">
                <h2><i class="fas fa-bullseye"></i> Current Focus</h2>
                <ul>
                    <li><span class="highlight">🔭 Working on:</span> Database Management Systems, AWS, Microsoft Technologies</li>
                    <li><span class="highlight">🌱 Learning:</span> React, Java, Spring Boot, React.js</li>
                    <li><span class="highlight">👯 Collaborating:</span> <a href="https://hesabook.com" style="color:#60a5fa;">School Management System - Hesabook</a></li>
                    <li><span class="highlight">✍️ Writing:</span> Articles on <a href="#" style="color:#60a5fa;">Artificial Intelligence</a></li>
                </ul>
                
                <div class="progress-container">
                    <div class="progress-title">
                        <span>React.js</span>
                        <span>1.5 years</span>
                    </div>
                    <div class="progress-bar">
                        <div class="progress-fill" style="width: 80%"></div>
                    </div>
                </div>
                
                <div class="progress-container">
                    <div class="progress-title">
                        <span>Java</span>
                        <span>1.5 years</span>
                    </div>
                    <div class="progress-bar">
                        <div class="progress-fill" style="width: 75%"></div>
                    </div>
                </div>
                
                <div class="progress-container">
                    <div class="progress-title">
                        <span>JavaScript</span>
                        <span>2 years</span>
                    </div>
                    <div class="progress-bar">
                        <div class="progress-fill" style="width: 90%"></div>
                    </div>
                </div>
            </div>
            
            <div class="card">
                <h2><i class="fas fa-user"></i> About Me</h2>
                <p>Passionate frontend developer with 1.5+ years of experience creating responsive and user-friendly web applications. I specialize in React ecosystem and modern JavaScript.</p>
                <p>I enjoy solving complex problems and turning ideas into reality through clean, efficient code. Constantly learning and exploring new technologies to stay at the forefront of web development.</p>
                
                <h3 style="margin-top: 1.5rem; color: #94a3b8;">Ask me about:</h3>
                <div class="skills-grid">
                    <div class="skill-item">
                        <i class="fab fa-react"></i>
                        <span>React</span>
                    </div>
                    <div class="skill-item">
                        <i class="fab fa-js"></i>
                        <span>JavaScript</span>
                    </div>
                    <div class="skill-item">
                        <i class="fab fa-html5"></i>
                        <span>HTML5</span>
                    </div>
                    <div class="skill-item">
                        <i class="fab fa-css3-alt"></i>
                        <span>CSS3</span>
                    </div>
                    <div class="skill-item">
                        <i class="fab fa-github"></i>
                        <span>GitHub</span>
                    </div>
                    <div class="skill-item">
                        <i class="fab fa-bitbucket"></i>
                        <span>Bitbucket</span>
                    </div>
                </div>
            </div>
        </div>
        
        <h2 class="section-title">Technical Skills</h2>
        
        <div class="focus-grid">
            <div class="focus-item">
                <i class="fas fa-code"></i>
                <h3>Frontend Development</h3>
                <p>React, Redux, JavaScript, HTML5, CSS3, Bootstrap, Tailwind CSS, React Native</p>
            </div>
            
            <div class="focus-item">
                <i class="fas fa-server"></i>
                <h3>Backend & Databases</h3>
                <p>Java, Spring Boot, Python, MySQL, MongoDB, Firebase</p>
            </div>
            
            <div class="focus-item">
                <i class="fas fa-tools"></i>
                <h3>Dev Tools & Platforms</h3>
                <p>Git, GitHub, Bitbucket, AWS, Babel, VS Code, IntelliJ</p>
            </div>
        </div>
        
        <h2 class="section-title">Connect With Me</h2>
        
        <div class="contact-grid">
            <div class="contact-item">
                <i class="fab fa-linkedin fa-2x"></i>
                <a href="https://linkedin.com/in/zeeshan-ahmad" target="_blank">LinkedIn</a>
            </div>
            
            <div class="contact-item">
                <i class="fab fa-instagram fa-2x"></i>
                <a href="https://instagram.com/itz_ahmed197" target="_blank">Instagram</a>
            </div>
            
            <div class="contact-item">
                <i class="fab fa-youtube fa-2x"></i>
                <a href="https://www.youtube.com/c/InterestingInfinity" target="_blank">YouTube</a>
            </div>
            
            <div class="contact-item">
                <i class="fas fa-laptop-code fa-2x"></i>
                <a href="https://www.codechef.com/users/zeeshan_Ahmad7" target="_blank">CodeChef</a>
            </div>
            
            <div class="contact-item">
                <i class="fas fa-envelope fa-2x"></i>
                <a href="mailto:za9414918@gmail.com">Email Me</a>
            </div>
        </div>
        
        <h2 class="section-title">GitHub Stats</h2>
        
        <div class="stats-container">
            <div class="stat-card">
                <h3>Profile Views</h3>
                <div class="stat-value">5.2K+</div>
                <p>Total profile visitors</p>
            </div>
            
            <div class="stat-card">
                <h3>Repositories</h3>
                <div class="stat-value">24</div>
                <p>Public projects</p>
            </div>
            
            <div class="stat-card">
                <h3>Contributions</h3>
                <div class="stat-value">1.2K+</div>
                <p>Last year activity</p>
            </div>
        </div>
        
        <footer>
            <p>© 2023 Zeeshan Ahmad | Passionate Frontend Developer</p>
            <p>Designed with ❤️ and ☕</p>
        </footer>
    </div>
</body>
</html>
