<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart House Price Forecasting | Data Science Solutions</title>
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            color: #333;
            background-color: #f9f9f9;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 1rem 0;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .container {
            width: 85%;
            max-width: 1200px;
            margin: auto;
            overflow: hidden;
            padding: 0 20px;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 2rem;
        }
        
        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
        }
        
        nav a:hover {
            color: var(--light-color);
        }
        
        .hero {
            padding: 3rem 0;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
        }
        
        .btn {
            display: inline-block;
            background: var(--accent-color);
            color: white;
            padding: 0.8rem 1.5rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            text-decoration: none;
            font-size: 1rem;
            transition: all 0.3s ease;
        }
        
        .btn:hover {
            background: #c0392b;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        section {
            padding: 3rem 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 2rem;
            color: var(--primary-color);
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .feature-card {
            background: white;
            padding: 2rem;
            border-radius: 5px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }
        
        .feature-card h3 {
            color: var(--secondary-color);
            margin-bottom: 1rem;
        }
        
        .algorithm-showcase {
            background: var(--light-color);
            padding: 3rem 0;
        }
        
        .algorithms {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }
        
        .algorithm {
            background: white;
            padding: 1.5rem;
            border-radius: 5px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .algorithm h3 {
            color: var(--primary-color);
            border-bottom: 2px solid var(--secondary-color);
            padding-bottom: 0.5rem;
            margin-bottom: 1rem;
        }
        
        .visualization {
            background: white;
            padding: 2rem;
            border-radius: 5px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            margin: 2rem 0;
        }
        
        .visualization img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }
        
        footer {
            background: var(--dark-color);
            color: white;
            text-align: center;
            padding: 2rem 0;
            margin-top: 2rem;
        }
        
        .contact-form {
            background: white;
            padding: 2rem;
            border-radius: 5px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            max-width: 600px;
            margin: 0 auto;
        }
        
        .form-group {
            margin-bottom: 1.5rem;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
        }
        
        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-family: inherit;
        }
        
        @media (max-width: 768px) {
            nav {
                flex-direction: column;
            }
            
            nav ul {
                margin-top: 1rem;
            }
            
            nav ul li {
                margin: 0 1rem;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <nav>
                <a href="#" class="logo">HousePriceAI</a>
                <ul>
                    <li><a href="#about">About</a></li>
                    <li><a href="#techniques">Techniques</a></li>
                    <li><a href="#demo">Demo</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
            
            <div class="hero">
                <h1>Smart House Price Forecasting</h1>
                <p>Leveraging advanced regression techniques and machine learning to predict real estate prices with unprecedented accuracy</p>
                <a href="#demo" class="btn">Try Our Demo</a>
            </div>
        </div>
    </header>
    
    <section id="about" class="about-section">
        <div class="container">
            <h2 class="section-title">About Our Price Forecasting Model</h2>
            <div class="features">
                <div class="feature-card">
                    <h3>Data-Driven Accuracy</h3>
                    <p>Our models analyze thousands of data points including location, square footage, amenities, market trends, and historical pricing to deliver accurate forecasts.</p>
                </div>
                <div class="feature-card">
                    <h3>Advanced Regression Techniques</h3>
                    <p>We employ ensemble methods combining linear regression, decision trees, and neural networks to capture both linear and non-linear relationships in housing data.</p>
                </div>
                <div class="feature-card">
                    <h3>Real-Time Market Adaptation</h3>
                    <p>Our system continuously learns from new transactions and market shifts, ensuring forecasts remain relevant in dynamic real estate environments.</p>
                </div>
            </div>
        </div>
    </section>
    
    <section id="techniques" class="algorithm-showcase">
        <div class="container">
            <h2 class="section-title">Regression Techniques We Use</h2>
            <div class="algorithms">
                <div class="algorithm">
                    <h3>Linear Regression</h3>
                    <p>The foundation of our model, establishing baseline relationships between house features and prices.</p>
                </div>
                <div class="algorithm">
                    <h3>Random Forest</h3>
                    <p>An ensemble method that reduces variance and improves prediction accuracy by combining multiple decision trees.</p>
                </div>
                <div class="algorithm">
                    <h3>Gradient Boosting</h3>
                    <p>Sequentially builds models to correct errors from previous iterations, excellent for handling complex patterns.</p>
                </div>
                <div class="algorithm">
                    <h3>Neural Networks</h3>
                    <p>Deep learning approach that captures intricate non-linear relationships in high-dimensional housing data.</p>
                </div>
            </div>
            
            <div class="visualization">
                <h3>Model Performance Comparison</h3>
                <img src="https://via.placeholder.com/800x400?text=Model+Accuracy+Comparison+Chart" alt="Model Accuracy Comparison">
                <p>Our hybrid approach consistently outperforms individual models across various evaluation metrics.</p>
            </div>
        </div>
    </section>
    
    <section id="demo" class="demo-section">
        <div class="container">
            <h2 class="section-title">Interactive Price Forecast Demo</h2>
            <div class="visualization">
                <img src="https://via.placeholder.com/800x500?text=Interactive+House+Price+Prediction+Tool" alt="Price Prediction Tool">
                <p>Enter property details to receive an instant price estimate powered by our machine learning models.</p>
            </div>
        </div>
    </section>
    
    <section id="contact" class="contact-section">
        <div class="container">
            <h2 class="section-title">Contact Our Data Science Team</h2>
            <div class="contact-form">
                <form>
                    <div class="form-group">
                        <label for="name">Name</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div class="form-group">
                        <label for="interest">Interest</label>
                        <select id="interest" name="interest">
                            <option value="forecasting">Price Forecasting</option>
                            <option value="partnership">Business Partnership</option>
                            <option value="research">Research Collaboration</option>
                            <option value="other">Other</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="message">Message</label>
                        <textarea id="message" name="message" rows="5" required></textarea>
                    </div>
                    <button type="submit" class="btn">Send Message</button>
                </form>
            </div>
        </div>
    </section>
    
    <footer>
        <div class="container">
            <p>&copy; 2023 HousePriceAI. All rights reserved.</p>
            <p>Advanced Data Science Solutions for Real Estate Forecasting</p>
        </div>
    </footer>
</body>
</html>
