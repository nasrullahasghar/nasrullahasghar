<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nasrullah Asghar - Data Scientist & AI Engineer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            line-height: 1.6;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: #ffffff;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            overflow: hidden;
        }

        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 60px 40px;
            text-align: center;
            position: relative;
        }

        .header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="%23ffffff" fill-opacity="0.1" d="M0,96L48,112C96,128,192,160,288,160C384,160,480,128,576,112C672,96,768,96,864,112C960,128,1056,160,1152,160C1248,160,1344,128,1392,112L1440,96L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>') no-repeat bottom;
            background-size: cover;
            opacity: 0.3;
        }

        .profile-image {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 6px solid rgba(255, 255, 255, 0.3);
            margin: 0 auto 20px;
            object-fit: cover;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            position: relative;
            z-index: 1;
        }

        h1 {
            font-size: 3em;
            margin-bottom: 10px;
            font-weight: 700;
            position: relative;
            z-index: 1;
        }

        .tagline {
            font-size: 1.3em;
            margin-bottom: 20px;
            opacity: 0.95;
            font-weight: 300;
            position: relative;
            z-index: 1;
        }

        .social-links {
            margin-top: 20px;
            position: relative;
            z-index: 1;
        }

        .social-links a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-size: 1.1em;
            padding: 10px 25px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 25px;
            display: inline-block;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .social-links a:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .content {
            padding: 50px 40px;
        }

        .section {
            margin-bottom: 50px;
        }

        .section-title {
            font-size: 2em;
            color: #667eea;
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 3px solid #667eea;
            display: inline-block;
        }

        .about-text {
            font-size: 1.15em;
            color: #555;
            line-height: 1.8;
            margin-bottom: 20px;
        }

        .highlight-box {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 30px;
            border-radius: 15px;
            margin: 20px 0;
            border-left: 5px solid #667eea;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 25px;
        }

        .skill-card {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 25px;
            border-radius: 15px;
            color: white;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }

        .skill-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
        }

        .skill-card h3 {
            font-size: 1.3em;
            margin-bottom: 15px;
            border-bottom: 2px solid rgba(255, 255, 255, 0.3);
            padding-bottom: 10px;
        }

        .skill-card ul {
            list-style: none;
        }

        .skill-card li {
            padding: 5px 0;
            padding-left: 20px;
            position: relative;
        }

        .skill-card li::before {
            content: '▹';
            position: absolute;
            left: 0;
            color: rgba(255, 255, 255, 0.7);
        }

        .focus-areas {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }

        .focus-item {
            background: white;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            border: 2px solid #667eea;
            transition: all 0.3s ease;
        }

        .focus-item:hover {
            background: #667eea;
            color: white;
            transform: scale(1.05);
        }

        .focus-item h4 {
            font-size: 1.1em;
            margin-bottom: 10px;
        }

        .cta-section {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px;
            text-align: center;
            border-radius: 15px;
            margin-top: 40px;
        }

        .cta-section h3 {
            font-size: 2em;
            margin-bottom: 20px;
        }

        .cta-button {
            display: inline-block;
            background: white;
            color: #667eea;
            padding: 15px 40px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1em;
            margin: 10px;
            transition: all 0.3s ease;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
            background: #f0f0f0;
        }

        .stats {
            display: flex;
            justify-content: space-around;
            margin: 30px 0;
            flex-wrap: wrap;
        }

        .stat-item {
            text-align: center;
            padding: 20px;
        }

        .stat-number {
            font-size: 2.5em;
            font-weight: 700;
            color: #667eea;
        }

        .stat-label {
            font-size: 1em;
            color: #666;
            margin-top: 5px;
        }

        @media (max-width: 768px) {
            h1 {
                font-size: 2em;
            }

            .tagline {
                font-size: 1.1em;
            }

            .content {
                padding: 30px 20px;
            }

            .skills-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>👋 Hi, I'm Nasrullah Asghar</h1>
            <p class="tagline">Data Scientist | AI/ML Engineer | Generative AI Enthusiast</p>
            <div class="social-links">
                <a href="https://linkedin.com/in/nasrullahasghar" target="_blank">🔗 LinkedIn</a>
                <a href="https://github.com/nasrullahasghar" target="_blank">💻 GitHub</a>
                <a href="nasrullahasghar897@gmail.com">📧 Email</a>
            </div>
        </div>

        <div class="content">
            <div class="section">
                <h2 class="section-title">About Me</h2>
                <p class="about-text">
                    I'm an aspiring Data Scientist and AI Engineer with a strong passion for leveraging artificial intelligence 
                    to solve real-world problems. My journey in data science is driven by curiosity and a commitment to continuous 
                    learning through hands-on projects and public knowledge sharing.
                </p>
                <p class="about-text">
                    Currently based in Lahore, Pakistan, I'm actively seeking opportunities in Data Science, Machine Learning Engineering, 
                    Generative AI, and Natural Language Processing. My approach combines theoretical understanding with practical 
                    implementation, focusing on building production-ready systems rather than toy datasets.
                </p>
                
                <div class="highlight-box">
                    <strong>🎯 Career Goal:</strong> To become a proficient AI/ML Engineer specializing in Generative AI and NLP, 
                    contributing to innovative solutions that make a meaningful impact.
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">Technical Expertise</h2>
                <div class="skills-grid">
                    <div class="skill-card">
                        <h3>🤖 Machine Learning & AI</h3>
                        <ul>
                            <li>Supervised & Unsupervised Learning</li>
                            <li>Deep Learning & Neural Networks</li>
                            <li>Natural Language Processing</li>
                            <li>Generative AI & LLMs</li>
                            <li>Model Deployment & MLOps</li>
                        </ul>
                    </div>

                    <div class="skill-card">
                        <h3>💻 Programming & Tools</h3>
                        <ul>
                            <li>Python (Pandas, NumPy, Scikit-learn)</li>
                            <li>TensorFlow & PyTorch</li>
                            <li>SQL & Database Management</li>
                            <li>Git & Version Control</li>
                            <li>Docker & Cloud Platforms</li>
                        </ul>
                    </div>

                    <div class="skill-card">
                        <h3>📊 Data Science</h3>
                        <ul>
                            <li>Exploratory Data Analysis</li>
                            <li>Statistical Analysis & Hypothesis Testing</li>
                            <li>Data Visualization (Matplotlib, Seaborn)</li>
                            <li>Feature Engineering</li>
                            <li>A/B Testing & Experimentation</li>
                        </ul>
                    </div>

                    <div class="skill-card">
                        <h3>🎯 Specialized Areas</h3>
                        <ul>
                            <li>Customer Segmentation & Retention</li>
                            <li>Demand Forecasting</li>
                            <li>NLP & Text Analytics</li>
                            <li>Uplift Modeling</li>
                            <li>End-to-End ML Systems</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">Core Focus Areas</h2>
                <div class="focus-areas">
                    <div class="focus-item">
                        <h4>🧠 Generative AI</h4>
                        <p>Building and fine-tuning LLMs for real-world applications</p>
                    </div>
                    <div class="focus-item">
                        <h4>📝 NLP Solutions</h4>
                        <p>Extracting insights from unstructured text data</p>
                    </div>
                    <div class="focus-item">
                        <h4>🚀 ML Engineering</h4>
                        <p>Deploying scalable production ML systems</p>
                    </div>
                    <div class="focus-item">
                        <h4>📈 Business Analytics</h4>
                        <p>Driving data-informed decision making</p>
                    </div>
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">Current Projects</h2>
                <div class="highlight-box">
                    <p><strong>🎯 Building a Hiring-Relevant Portfolio</strong></p>
                    <p>I'm currently working on five comprehensive data science projects that demonstrate real-world skills:</p>
                    <ul style="margin-top: 15px; margin-left: 20px;">
                        <li>📊 Customer Segmentation & Retention Analysis</li>
                        <li>📈 Demand Forecasting System</li>
                        <li>💬 NLP Insights from Unstructured Data</li>
                        <li>🧪 Experimentation & Uplift Modeling</li>
                        <li>⚙️ End-to-End ML System with Deployment</li>
                    </ul>
                </div>
            </div>

            <div class="section">
                <h2 class="section-title">My Approach</h2>
                <div class="stats">
                    <div class="stat-item">
                        <div class="stat-number">📚</div>
                        <div class="stat-label">Public Learning</div>
                    </div>
                    <div class="stat-item">
                        <div class="stat-number">🛠️</div>
                        <div class="stat-label">Project-Based Growth</div>
                    </div>
                    <div class="stat-item">
                        <div class="stat-number">🌐</div>
                        <div class="stat-label">Community Engagement</div>
                    </div>
                    <div class="stat-item">
                        <div class="stat-number">💡</div>
                        <div class="stat-label">Continuous Learning</div>
                    </div>
                </div>
                <p class="about-text" style="text-align: center;">
                    I believe in learning in public, sharing knowledge through daily content creation, and building 
                    a strong professional presence on LinkedIn. Every project is an opportunity to learn, grow, and 
                    contribute to the data science community.
                </p>
            </div>

            <div class="cta-section">
                <h3>Let's Connect! 🤝</h3>
                <p style="margin-bottom: 25px; font-size: 1.1em;">
                    I'm actively seeking opportunities in Data Science, ML Engineering, and Generative AI roles in Lahore. 
                    Open to collaborations, mentorship, and exciting projects!
                </p>
                <a href="https://linkedin.com/in/nasrullahasghar" class="cta-button" target="_blank">Connect on LinkedIn</a>
                <a href="mailto:your.email@example.com" class="cta-button">Send Email</a>
            </div>

            <div style="text-align: center; margin-top: 40px; color: #999; font-size: 0.9em;">
                <p>⚡ Fun Fact: I'm an avid cricket lover! 🏏</p>
                <p style="margin-top: 10px;">📍 Based in Lahore, Pakistan | 🌟 Pronouns: He/Him</p>
            </div>
        </div>
    </div>
</body>
</html>
