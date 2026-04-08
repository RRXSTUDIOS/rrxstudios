<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>RRX STUDIOS | Innovation in Motion</title>
    <style>
        :root {
            --primary-color: #FFD700;
            --bg-dark: #0a0a0a;
            --card-bg: #161616;
            --text-light: #ffffff;
            --nav-height: 70px;
        }

        * {
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Roboto, sans-serif;
            background-color: var(--bg-dark);
            color: var(--text-light);
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        /* --- Mobile Optimized Navbar --- */
        nav {
            display: flex;
            justify-content: center; /* মোবাইলে লোগো মাঝখানে রাখার জন্য */
            align-items: center;
            padding: 0 20px;
            height: var(--nav-height);
            background: rgba(0, 0, 0, 0.9);
            backdrop-filter: blur(12px);
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 10000;
            border-bottom: 1px solid rgba(255, 215, 0, 0.1);
        }

        .logo {
            font-size: 1.3rem;
            font-weight: 800;
            color: var(--primary-color);
            letter-spacing: 3px;
            text-transform: uppercase;
        }

        /* --- Hero Section (Responsive) --- */
        .hero {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 20px;
            background: radial-gradient(circle at center, #1a1a1a 0%, #000000 100%);
        }

        .hero h1 {
            font-size: clamp(2rem, 10vw, 4.5rem); /* স্ক্রিন অনুযায়ী অটো সাইজ হবে */
            margin-bottom: 15px;
            letter-spacing: 5px;
            font-weight: 900;
        }

        .hero p {
            font-size: clamp(0.9rem, 4vw, 1.2rem);
            color: #888;
            margin-bottom: 35px;
            max-width: 600px;
        }

        .cta-btn {
            padding: 14px 35px;
            background-color: var(--primary-color);
            color: #000;
            text-decoration: none;
            font-weight: bold;
            border-radius: 50px;
            font-size: 1rem;
            transition: 0.3s;
            box-shadow: 0 5px 15px rgba(255, 215, 0, 0.2);
        }

        /* --- Expertise Section (Mobile Grid) --- */
        .about {
            padding: 80px 20px;
            max-width: 1200px;
            margin: 0 auto;
            text-align: center;
        }

        .about h2 {
            color: var(--primary-color);
            font-size: clamp(1.8rem, 6vw, 2.5rem);
            margin-bottom: 40px;
        }

        .grid {
            display: grid;
            grid-template-columns: 1fr; /* মোবাইলে এক কলাম */
            gap: 20px;
        }

        /* ট্যাবলেট বা পিসিতে ৩ কলাম হবে */
        @media (min-width: 768px) {
            .grid { grid-template-columns: repeat(3, 1fr); }
            nav { justify-content: space-between; padding: 0 10%; }
        }

        .card {
            background: var(--card-bg);
            padding: 35px 25px;
            border-radius: 20px;
            border: 1px solid #222;
            transition: 0.3s ease;
        }

        .card:active { transform: scale(0.98); } /* মোবাইলে টাচ করলে হালকা ছোট হবে */

        .card h3 {
            color: var(--primary-color);
            margin-top: 0;
            font-size: 1.4rem;
        }

        .card p {
            color: #bbb;
            font-size: 0.95rem;
            margin-bottom: 0;
        }

        footer {
            padding: 40px 20px;
            text-align: center;
            font-size: 0.8rem;
            color: #444;
            border-top: 1px solid #111;
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">RRX STUDIOS</div>
    </nav>

    <section class="hero">
        <h1>RRX STUDIOS</h1>
        <p>Innovation in Motion | Leading the Digital Frontier</p>
        <a href="#about" class="cta-btn">Explore Studio</a>
    </section>

    <section id="about" class="about">
        <h2>Our Expertise</h2>
        <div class="grid">
            <div class="card">
                <h3>Digital Content</h3>
                <p>High-end video production and immersive gaming content for the modern audience.</p>
            </div>
            <div class="card">
                <h3>Innovation</h3>
                <p>Harnessing latest technology to create smart and scalable digital ecosystems.</p>
            </div>
            <div class="card">
                <h3>Branding</h3>
                <p>Designing powerful visual identities that resonate with global standards.</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 RRX STUDIOS | Powered by Innovation</p>
    </footer>

</body>
</html>
