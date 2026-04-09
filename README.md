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
            --bg-dark: #08020d; /* Deep Dark Violet */
            --card-bg: rgba(20, 20, 20, 0.7);
            --text-light: #ffffff;
            --discord: #5865F2;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: 'Rajdhani', sans-serif;
            background-color: var(--bg-dark);
            background-image: radial-gradient(circle, rgba(255, 49, 49, 0.1) 1px, transparent 1px);
            background-size: 30px 30px; /* Dot pattern like logo */
            color: var(--text-light);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        /* --- Navbar --- */
        nav {
            display: flex; justify-content: space-between; align-items: center;
            padding: 0 8%; height: 80px;
            background: rgba(8, 2, 13, 0.9); backdrop-filter: blur(10px);
            position: fixed; top: 0; width: 100%; z-index: 1000;
            border-bottom: 1px solid var(--rrx-red);
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

        /* --- Hero Section --- */
        .hero {
            height: 100vh; display: flex; flex-direction: column;
            justify-content: center; align-items: center; text-align: center;
            background: radial-gradient(circle at center, var(--rrx-purple) -100%, var(--bg-dark) 80%);
        }

        /* Logo-style Glitch Effect */
        .glitch-title {
            font-family: 'Orbitron', sans-serif;
            font-size: clamp(3rem, 12vw, 6rem);
            font-weight: 900;
            position: relative;
            color: white;
            text-transform: uppercase;
            letter-spacing: 10px;
        }

        .glitch-title::before, .glitch-title::after {
            content: "RRX STUDIOS";
            position: absolute; top: 0; left: 0; width: 100%; height: 100%;
        }

        .glitch-title::before {
            left: 2px; text-shadow: -2px 0 var(--rrx-red);
            clip: rect(44px, 450px, 56px, 0);
            animation: glitch-anim 5s infinite linear alternate-reverse;
        }

        .glitch-title::after {
            left: -2px; text-shadow: -2px 0 var(--rrx-purple);
            clip: rect(44px, 450px, 56px, 0);
            animation: glitch-anim2 5s infinite linear alternate-reverse;
        }

        @keyframes glitch-anim {
            0% { clip: rect(10px, 9999px, 20px, 0); }
            20% { clip: rect(30px, 9999px, 40px, 0); }
            100% { clip: rect(80px, 9999px, 90px, 0); }
        }

        @keyframes glitch-anim2 {
            0% { clip: rect(60px, 9999px, 70px, 0); }
            50% { clip: rect(20px, 9999px, 30px, 0); }
            100% { clip: rect(10px, 9999px, 25px, 0); }
        }

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

        /* --- Expertise Section --- */
        .section { padding: 100px 8%; text-align: center; }
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; margin-top: 50px; }

        .card {
            background: var(--card-bg); padding: 40px; border-radius: 15px;
            border: 1px solid rgba(255, 49, 49, 0.2); transition: 0.4s;
            backdrop-filter: blur(5px);
        }
        .card:hover {
            border-color: var(--rrx-red);
            transform: scale(1.05);
            box-shadow: 0 10px 30px rgba(255, 49, 49, 0.2);
        }
        .card h3 { color: var(--rrx-red); margin-bottom: 15px; font-family: 'Orbitron'; }

        /* --- Footer --- */
        footer { padding: 50px; text-align: center; border-top: 1px solid #222; }
        .copyright { color: #444; font-size: 0.8rem; margin-top: 20px; }

    </style>
</head>
<body>

    <nav>
        <div class="logo">RRX STUDIOS</div>
        <div class="nav-links">
            <a href="#">Home</a>
            <a href="#expertise">Expertise</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <section class="hero">
        <h1 class="glitch-title">RRX STUDIOS</h1>
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
                <h3>Digital Content</h3>
                <p>High-fidelity video production and immersive storytelling.</p>
            </div>
            <div class="card">
                <h3>Innovation</h3>
                <p>Designing the next generation of digital ecosystems.</p>
            </div>
            <div class="card">
                <h3>Brand Identity</h3>
                <p>Creating visual legacies that dominate the industry.</p>
            </div>
        </div>
    </section>

    <footer>
        <p style="color: var(--rrx-red); font-family: 'Orbitron';">RRX NETWORK</p>
        <p class="copyright">&copy; 2026 RRX STUDIOS | POWERED BY REDRROX</p>
    </footer>

</body>
</html>
