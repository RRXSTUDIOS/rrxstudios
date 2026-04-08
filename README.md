<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RRX STUDIOS | Innovation in Motion</title>
    <style>
        :root {
            --primary-color: #FFD700;
            --bg-dark: #0a0a0a;
            --card-bg: #161616;
            --text-light: #ffffff;
            --nav-height: 70px;
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Roboto, sans-serif;
            background-color: var(--bg-dark);
            color: var(--text-light);
            scroll-behavior: smooth;
        }

        /* --- Navbar --- */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 10%;
            height: var(--nav-height);
            background: rgba(0, 0, 0, 0.95);
            backdrop-filter: blur(10px);
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 10000;
            border-bottom: 1px solid rgba(255, 215, 0, 0.1);
            box-sizing: border-box;
        }

        .logo {
            font-size: 1.3rem;
            font-weight: 800;
            color: var(--primary-color);
            letter-spacing: 2px;
            text-transform: uppercase;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
            font-size: 0.9rem;
            transition: 0.3s;
        }

        .nav-links a:hover { color: var(--primary-color); }

        /* --- Hero Section --- */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: radial-gradient(circle, #1a1a1a 0%, #000000 100%);
        }

        .hero h1 {
            font-size: clamp(2.5rem, 8vw, 5rem);
            margin-bottom: 10px;
            letter-spacing: 5px;
        }

        /* --- Expertise Section & ANIMATION --- */
        .section { padding: 100px 10%; text-align: center; }
        
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .card {
            background: var(--card-bg);
            padding: 40px 30px;
            border-radius: 20px;
            border: 1px solid #222;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); /* Smooth Slide/Pop Effect */
            position: relative;
            overflow: hidden;
        }

        /* HOVER ANIMATION HERE */
        .card:hover {
            transform: translateY(-15px); /* Upward Slide */
            border-color: var(--primary-color);
            box-shadow: 0 15px 30px rgba(255, 215, 0, 0.1);
        }

        .card h3 { color: var(--primary-color); margin-bottom: 15px; }

        /* --- Contact Section --- */
        .contact-box {
            background: var(--card-bg);
            padding: 40px;
            border-radius: 20px;
            display: inline-block;
            margin-top: 30px;
        }

        .contact-box a {
            color: var(--primary-color);
            text-decoration: none;
            font-weight: bold;
            font-size: 1.2rem;
        }

        /* --- Footer & Links --- */
        footer {
            padding: 60px 10%;
            background: #000;
            border-top: 1px solid #111;
            text-align: center;
        }

        .footer-links { margin-bottom: 20px; }
        .footer-links a {
            color: #888;
            text-decoration: none;
            margin: 0 15px;
            font-size: 0.9rem;
            transition: 0.3s;
        }
        .footer-links a:hover { color: var(--primary-color); }

        @media (max-width: 768px) {
            .nav-links { display: none; } /* Mobile a menu hide kora hoyeche simplified rakhar jonno */
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">RRX STUDIOS</div>
        <div class="nav-links">
            <a href="#">Home</a>
            <a href="#about">Expertise</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <section class="hero">
        <h1>RRX STUDIOS</h1>
        <p>Innovation in Motion</p>
    </section>

    <section id="about" class="section">
        <h2 style="color: var(--primary-color); font-size: 2.5rem;">Our Expertise</h2>
        <div class="grid">
            <div class="card">
                <h3>Digital Content</h3>
                <p>Creating high-end video production and immersive gaming narratives.</p>
            </div>
            <div class="card">
                <h3>Innovation</h3>
                <p>Developing future-ready digital solutions with cutting-edge tech.</p>
            </div>
            <div class="card">
                <h3>Brand Identity</h3>
                <p>Designing powerful visual identities that dominate the market.</p>
            </div>
        </div>
    </section>

    <section id="contact" class="section" style="background: #0f0f0f;">
        <h2 style="color: var(--primary-color);">Get In Touch</h2>
        <p>আমাদের সাথে যোগাযোগ করতে বা প্রজেক্ট নিয়ে আলোচনা করতে ইমেইল করুন।</p>
        <div class="contact-box">
            <a href="mailto:contact.rrxstudios@gmail.com">contact.rrxstudios@gmail.com</a>
        </div>
    </section>

    <footer>
        <div class="footer-links">
            <strong>Our Ventures:</strong><br><br>
            <a href="https://rrxstudios.github.io/RRX/">RRX Studios v3</a>
            <a href="https://rrxstudios.github.io/RRX/">RRX Studios v4</a>
            <a href="https://rrxstudios.github.io/RRX/">RRX Studios v5</a>
        </div>
        <p>&copy; 2026 RRX STUDIOS | Powered by Innovation</p>
    </footer>

</body>
</html>
