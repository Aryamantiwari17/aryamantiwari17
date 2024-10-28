<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <style>
        :root {
            --primary-color: #0366d6;
            --text-color: #24292e;
            --bg-color: #ffffff;
            --secondary-bg: #f6f8fa;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
            background: var(--bg-color);
        }

        .header {
            text-align: center;
            margin-bottom: 2rem;
        }

        .title {
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 0.5rem;
        }

        .subtitle {
            font-size: 1.2rem;
            color: #586069;
        }

        .section {
            margin: 2rem 0;
            padding: 1rem;
            border-radius: 6px;
            background: var(--secondary-bg);
        }

        .project-card {
            background: var(--bg-color);
            border: 1px solid #e1e4e8;
            border-radius: 6px;
            padding: 1rem;
            margin: 1rem 0;
            transition: transform 0.2s;
        }

        .project-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        }

        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .skill-tag {
            background: #e1e4e8;
            padding: 0.3rem 0.8rem;
            border-radius: 15px;
            font-size: 0.9rem;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 2rem;
        }

        .social-link {
            color: var(--primary-color);
            text-decoration: none;
            padding: 0.5rem 1rem;
            border: 1px solid var(--primary-color);
            border-radius: 4px;
            transition: all 0.2s;
        }

        .social-link:hover {
            background: var(--primary-color);
            color: white;
        }

        .achievements {
            list-style: none;
            padding: 0;
        }

        .achievements li {
            margin: 0.5rem 0;
            padding-left: 1.5rem;
            position: relative;
        }

        .achievements li::before {
            content: "🏆";
            position: absolute;
            left: 0;
        }

        @media (prefers-color-scheme: dark) {
            :root {
                --primary-color: #58a6ff;
                --text-color: #c9d1d9;
                --bg-color: #0d1117;
                --secondary-bg: #161b22;
            }

            .project-card {
                border-color: #30363d;
            }

            .skill-tag {
                background: #21262d;
            }
        }
    </style>
</head>
<body>
    <div class="header">
        <h1 class="title">Aryaman Tiwari</h1>
        <p class="subtitle">🚀 Machine Learning | AI | NLP | Data Science Enthusiast</p>
    </div>

    <div class="section">
        <p>Welcome! I'm a final-year B.Tech student in Computer Science at Jaypee University of Information Technology, actively pushing boundaries in AI, machine learning, and NLP. My journey has been marked by hands-on projects, transformative internships, and open-source contributions—all geared toward making a meaningful impact with technology.</p>
    </div>

    <div class="section">
        <h2>📍 Current Focus</h2>
        <ul>
            <li><strong>Generative AI:</strong> Learning from Krish Naik, India's prominent LLM mentor</li>
            <li><strong>Open Source Contribution:</strong> Building on my skills by contributing to Milvus, a leading vector database</li>
        </ul>
    </div>

    <div class="section">
        <h2>🌟 Featured Projects</h2>
        <div class="project-card">
            <h3>Nutri_BOT 🍎</h3>
            <p><strong>AI-powered Nutrition Analyzer:</strong> Extracts and analyzes nutritional data from food product images using OCR and Gemini AI for accurate health insights.</p>
            <div class="skills-container">
                <span class="skill-tag">OCR</span>
                <span class="skill-tag">Gemini AI</span>
            </div>
        </div>

        <div class="project-card">
            <h3>Predicting Next Word Using LSTM_GRU 🔮</h3>
            <p><strong>Intelligent Word Predictor:</strong> A Streamlit app that suggests the next word based on user input, using a pre-trained LSTM model for smart text completion.</p>
            <div class="skills-container">
                <span class="skill-tag">TensorFlow</span>
                <span class="skill-tag">Keras</span>
                <span class="skill-tag">Streamlit</span>
            </div>
        </div>

        <!-- Add more project cards as needed -->
    </div>

    <div class="section">
        <h2>🛠️ Skills</h2>
        <div class="skills-container">
            <span class="skill-tag">Python</span>
            <span class="skill-tag">C++</span>
            <span class="skill-tag">JavaScript</span>
            <span class="skill-tag">TensorFlow</span>
            <span class="skill-tag">Keras</span>
            <span class="skill-tag">Flask</span>
            <span class="skill-tag">FastAPI</span>
            <span class="skill-tag">LangChain</span>
        </div>
    </div>

    <div class="section">
        <h2>🏆 Honors & Achievements</h2>
        <ul class="achievements">
            <li><strong>IEEE Hackathon</strong> - Placed 3rd out of 200 for a solution to reduce crime in Venezuela</li>
            <li><strong>Campus Ambassador at EDC IIT Delhi</strong> - Networked with top entrepreneurs and industry leaders</li>
            <li><strong>Top LeetCode Coder</strong> - Solved 50+ problems in a month, achieving 4-star ranking on HackerRank for Python</li>
        </ul>
    </div>

    <div class="social-links">
        <a href="https://github.com/aryamantiwari" class="social-link">GitHub</a>
        <a href="https://linkedin.com/in/aryamantiwari" class="social-link">LinkedIn</a>
        <a href="https://leetcode.com/aryamantiwari02" class="social-link">LeetCode</a>
        <a href="mailto:aryamantiwari02@gmail.com" class="social-link">Email</a>
    </div>

    <script>
        // Add smooth scrolling to all links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Add animation to project cards on scroll
        const observerOptions = {
            threshold: 0.1
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.project-card').forEach(card => {
            card.style.opacity = '0';
            card.style.transform = 'translateY(20px)';
            card.style.transition = 'all 0.5s ease-out';
            observer.observe(card);
        });
    </script>
</body>
</html>
