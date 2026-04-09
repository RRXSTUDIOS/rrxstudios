<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RRX STUDIOS | Innovation in Motion</title>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;900&family=Rajdhani:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --rrx-red: #ff3131;
            --rrx-purple: #4e148c;
            --bg-dark: #08020d; /* Deep Dark Violet like logo background */
            --card-bg: rgba(20, 20, 20, 0.7);
            --text-light: #ffffff;
            --discord: #5865F2;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: 'Rajdhani', sans-serif;
            background-color: var(--bg-dark);
            background-image: radial-gradient(circle, rgba(255, 49, 49, 0.1) 1px, transparent 1px);
            background-size: 30px 30px; /* Dot pattern from logo */
            color: var(--text-light);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        /* --- Navbar --- */
        nav {
            display: flex; justify-content: space-between; align-items: center;
            padding: 0 8%; height: 80px;
            background: rgba(8, 2, 13, 0.95); backdrop-filter: blur(10px);
            position: fixed; top: 0; width: 100%; z-index: 1000;
            border-bottom: 2px solid var(--rrx-red);
        }

        .logo {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.5rem; font-weight: 900;
            color: white; letter-spacing: 2px;
            text-shadow: 2px 0 var(--rrx-red), -2px 0 var(--rrx-purple);
        }

        .nav-links a {
            color: #ccc; text-decoration: none; margin-left: 25px;
            font-weight: 700; text-transform: uppercase; transition: 0.3s;
        }
        .nav-links a:hover { color: var(--rrx-red); }

        /* --- Hero Section with Gears --- */
        .hero {
            height: 100vh; display: flex; flex-direction: column;
            justify-content: center; align-items: center; text-align: center;
            background: radial-gradient(circle at center, var(--rrx-purple) -100%, var(--bg-dark) 80%);
            position: relative; overflow: hidden;
        }

        /* Floating gears animation from logo theme */
        .hero-gear {
            position: absolute; color: rgba(255, 49, 49, 0.1);
            font-size: 10rem; animation: rotate 20s infinite linear;
        }
        .hero-gear-1 { top: -10%; left: -5%; }
        .hero-gear-2 { bottom: -10%; right: -5%; font-size: 15rem; }

        @keyframes rotate { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }

        .glitch-title {
            font-family: 'Orbitron', sans-serif;
            font-size: clamp(3rem, 12vw, 6rem);
            font-weight: 900;
            position: relative;
            color: white;
            text-transform: uppercase;
            letter-spacing: 10px;
            text-shadow: 3px 3px 10px var(--rrx-red); /* Glowing Title */
        }
        
        /* Gears around title */
        .title-gear { font-size: 2rem; color: var(--rrx-red); vertical-align: middle; margin: 0 10px; }

        .hero p {
            font-family: 'Orbitron', sans-serif;
            letter-spacing: 5px; color: #888;
            margin-bottom: 30px; font-weight: 500;
        }

        /* --- Buttons --- */
        .social-group { display: flex; gap: 20px; }
        .btn {
            padding: 12px 30px; border-radius: 5px; text-decoration: none;
            font-family: 'Orbitron', sans-serif; font-weight: 700;
            transition: 0.4s; border: 2px solid var(--rrx-red); color: white;
        }
        .btn:hover {
            background: var(--rrx-red);
            box-shadow: 0 0 20px var(--rrx-red);
            transform: translateY(-3px);
        }

        .discord-btn { border-color: var(--discord); color: var(--discord); }
        .discord-btn:hover { background: var(--discord); color: white; box-shadow: 0 0 20px var(--discord); }

        /* --- Expertise Section with Cards Gears --- */
        .section { padding: 100px 8%; text-align: center; }
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; margin-top: 50px; }

        .card {
            background: var(--card-bg); padding: 40px; border-radius: 15px;
            border: 1px solid rgba(255, 49, 49, 0.2); transition: 0.4s;
            backdrop-filter: blur(5px);
            position: relative;
        }
        .card:hover {
            border-color: var(--rrx-red);
            transform: scale(1.05);
            box-shadow: 0 10px 30px rgba(255, 49, 49, 0.2);
        }
        /* Gear icon inside cards */
        .card-gear { position: absolute; top: -15px; left: -15px; font-size: 3rem; color: rgba(255, 49, 49, 0.2); }
        .card:hover .card-gear { color: var(--rrx-red); animation: rotate 5s infinite linear; }
        .card h3 { color: var(--rrx-red); margin-bottom: 15px; font-family: 'Orbitron'; }

        /* --- Contact & CORE Section (Restored) --- */
        .contact-core { padding: 80px 8%; text-align: center; background: #050109; border-top: 1px solid #111; }
        .contact-container {
            display: flex; justify-content: space-around; flex-wrap: wrap; gap: 30px; margin-top: 50px;
        }
        .core-card, .mail-card {
            background: var(--card-bg); padding: 30px; border-radius: 15px;
            border: 1px solid rgba(255, 49, 49, 0.2);
            flex: 1; min-width: 300px;
        }
        .core-card h4, .mail-card h4 { color: white; font-family: 'Orbitron'; margin-bottom: 15px; }
        .core-link, .mail-link { color: var(--rrx-red); text-decoration: none; font-weight: bold; font-size: 1.2rem; }
        .mail-link { word-break: break-all; }

        /* --- Footer with Glow --- */
        footer { padding: 50px; text-align: center; border-top: 1px solid #111; background: #020005; }
        .footer-network { color: white; font-family: 'Orbitron'; font-weight: 700; letter-spacing: 2px; }
        /* © Glow Effect */
        .copyright {
            color: rgba(255, 49, 49, 0.8);
            font-size: 0.8rem; margin-top: 20px;
            font-family: 'Rajdhani', sans-serif;
            text-transform: uppercase; letter-spacing: 1px;
            text-shadow: 0 0 10px var(--rrx-red), 0 0 5px var(--rrx-red);
        }

    </style>
</head>
<body>

    <nav>
        <div class="logo">RRX STUDIOS</div>
        <div class="nav-links">
            <a href="#">Home</a>
            <a href="#expertise">Expertise</a>
            <a href="#contact-core">Network</a>
        </div>
    </nav>

    <section class="hero">
        <div class="hero-gear hero-gear-1">⚙️</div>
        <div class="hero-gear hero-gear-2">⚙️</div>
        <h1 class="glitch-title"><span class="title-gear">⚙️</span>RRX STUDIOS<span class="title-gear">⚙️</span></h1>
        <p>Innovation in Motion</p>
        
        <div class="social-group">
            <a href="#" class="btn">YouTube</a>
            <a href="https://discord.gg/vGKpaZdFtt" target="_blank" class="btn discord-btn">Discord</a>
        </div>
    </section>

    <section id="expertise" class="section">
        <h2 style="font-family: 'Orbitron'; letter-spacing: 5px;">OUR EXPERTISE</h2>
        <div class="grid">
            <div class="card">
                <div class="card-gear">⚙️</div>
                <h3>Digital Content</h3>
                <p>High-fidelity video production and immersive storytelling.</p>
            </div>
            <div class="card">
                <div class="card-gear">⚙️</div>
                <h3>Innovation</h3>
                <p>Designing the next generation of digital ecosystems.</p>
            </div>
            <div class="card">
                <div class="card-gear">⚙️</div>
                <h3>Brand Identity</h3>
                <p>Creating visual legacies that dominate the industry.</p>
            </div>
        </div>
    </section>

    <section id="contact-core" class="contact-core">
        <h2 style="font-family: 'Orbitron'; letter-spacing: 5px;">RRX SUPPORT & CORE</h2>
        <div class="contact-container">
            <div class="core-card">
                <h4>GAMING CORE</h4>
                <p style="color: #666; margin-bottom: 10px;">Premium Digital Goods Market</p>
                <a href="https://rrxstudios.github.io/RRXCORE/" target="_blank" class="core-link">RRXCORE Market</a>
            </div>
            <div class="mail-card">
                <h4>SUPPORT MAIL</h4>
                <p style="color: #666; margin-bottom: 10px;">Official Brand Contact</p>
                <a href="mailto:rrxstudiosofficial@gmail.com" class="mail-link">rrxstudiosofficial@gmail.com</a>
            </div>
        </div>
    </section>

    <footer>
        <p class="footer-network">RRX NETWORK</p>
        <p class="copyright">&copy; 2026 RRX STUDIOS | POWERED BY REDRROX</p>
    </footer>

</body>
</html>
