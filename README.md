<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stylelix Portfolio</title>
    <style>
        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Basic Styles */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            scroll-behavior: smooth;
        }

        header {
            background: #333;
            color: #fff;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }

        .nav-links {
            list-style: none;
            display: flex;
        }

        .nav-links li {
            margin-left: 2rem;
        }

        .nav-links a {
            color: #fff;
            text-decoration: none;
            font-size: 1rem;
            position: relative;
        }

        .nav-links a::after {
            content: '';
            display: block;
            width: 0;
            height: 2px;
            background: #007BFF;
            transition: width 0.3s;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .hero-section {
            background: url('your-hero-image.jpg') no-repeat center center/cover;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            margin-top: 70px;
        }

        .hero-content h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            animation: fadeIn 2s ease-in-out;
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            animation: fadeIn 2s ease-in-out 1s;
        }

        .btn {
            background: #007BFF;
            color: #fff;
            padding: 0.8rem 1.2rem;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s ease;
            animation: fadeIn 2s ease-in-out 2s;
        }

        .btn:hover {
            background: #0056b3;
        }

        .about-section, .portfolio-section, .contact-section {
            padding: 4rem 2rem;
            text-align: center;
        }

        .about-section img {
            max-width: 300px;
            margin-top: 2rem;
            border-radius: 50%;
            animation: fadeIn 2s ease-in-out;
        }

        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .portfolio-item {
            animation: fadeIn 2s ease-in-out;
        }

        .portfolio-item video {
            width: 100%;
            border-radius: 10px;
        }

        form {
            display: flex;
            flex-direction: column;
            max-width: 600px;
            margin: 0 auto;
            animation: fadeIn 2s ease-in-out;
        }

        form input, form textarea {
            padding: 1rem;
            margin-bottom: 1rem;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        form button {
            background: #007BFF;
            color: #fff;
            padding: 1rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        form button:hover {
            background: #0056b3;
        }

        footer {
            background: #333;
            color: #fff;
            text-align: center;
            padding: 1rem 0;
        }

        /* Animations */
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">MyPortfolio</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero-section">
        <div class="hero-content">
            <h1>Welcome to My Editing Portfolio</h1>
            <p>Discover my work and projects</p>
            <a href="#portfolio" class="btn">View Portfolio</a>
        </div>
    </section>

    <section id="about" class="about-section">
        <h2>About Me</h2>
        <p>Hello! I'm an editor with a passion for creating captivating content.</p>
        <img src="your-image.jpg" alt="About Me">
    </section>

    <section id="portfolio" class="portfolio-section">
        <h2>My Work</h2>
        <div class="portfolio-grid">
            <div class="portfolio-item">
                <video controls>
                    <source src="your-video.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                </video>
                <p>Project Description</p>
            </div>
            <!-- Add more portfolio items as needed -->
        </div>
    </section>

    <section id="contact" class="contact-section">
        <h2>Contact Me</h2>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" required></textarea>
            <button type="submit">Send</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 fortnitre. All rights reserved.</p>
    </footer>
</body>
</html>
