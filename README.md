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
            --bg-dark: #08020d;
            --card-bg: rgba(20, 20, 20, 0.7);
            --text-light: #ffffff;
            --discord: #5865F2;
            --youtube: #ff0000;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: 'Rajdhani', sans-serif;
            background-color: var(--bg-dark);
            background-image: radial-gradient(circle, rgba(255, 49, 49, 0.1) 1px, transparent 1px);
            background-size: 30px 30px;
            color: var(--text-light);
            overflow-x: hidden; /* স্ক্রিন ডানে সরবে না */
            scroll-behavior: smooth;
            width: 100%;
        }

        /* --- Navbar Fix (সব বামে এবং স্ক্রিনের ভেতরে) --- */
        nav {
            height: 75px;
            background: rgba(8, 2, 13, 0.98);
            backdrop-filter: blur(15px);
            position: fixed; top: 0; width: 100%; z-index: 10000;
            border-bottom: 2px solid var(--rrx-red);
            display: flex;
            align-items: center;
            padding: 0 5%;
        }

        .logo {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.3rem; font-weight: 900;
            color: white; letter-spacing: 2px;
            text-shadow: 2px 0 var(--rrx-red);
            margin-right: 30px;
            flex-shrink: 0;
        }

        .nav-links { 
            display: flex; 
            gap: 15px;
        } 
        .nav-links a {
            color: #ccc; text-decoration: none;
            font-size: 0.8rem; font-weight: 700; text-transform: uppercase; transition: 0.3s;
        }
        .nav-links a:hover { color: var(--rrx-red); }

        /* --- Hero Section --- */
        .hero {
            height: 100vh; display: flex; flex-direction: column;
            justify-content: center; align-items: center; text-align: center;
            background: radial-gradient(circle at center, var(--rrx-purple) -100%, var(--bg-dark) 80%);
            position: relative; overflow: hidden; padding: 20px;
        }

        .hero-gear {
            position: absolute; color: rgba(255, 49, 49, 0.05);
            font-size: 10rem; animation: rotate 20s infinite linear; z-index: 0;
        }
        .hero-gear-1 { top: -5%; left: -5%; }
        .hero-gear-2 { bottom: -5%; right: -5%; font-size: 15rem; }

        @keyframes rotate { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }

        .glitch-title {
            font-family: 'Orbitron', sans-serif;
            font-size: clamp(2.5rem, 10vw, 5.5rem);
            font-weight: 900; position: relative; color: white;
            text-transform: uppercase; letter-spacing: 5px;
            text-shadow: 0 0 15px var(--rrx-red); z-index: 1;
        }

        .hero p {
            font-family: 'Orbitron', sans-serif; letter-spacing: 4px;
            color: #888; margin-top: 10px; margin-bottom: 30px; font-weight: 500; z-index: 1;
        }

        /* --- Social Buttons --- */
        .social-group { display: flex; gap: 15px; flex-wrap: wrap; justify-content: center; z-index: 1; }
        .btn-social {
            padding: 12px 28px; border-radius: 50px; text-decoration: none;
            font-family: 'Orbitron', sans-serif; font-weight: 700; font-size: 0.9rem;
            transition: 0.4s; display: flex; align-items: center; gap: 10px; border: 2px solid transparent;
        }
        .youtube-btn { background: rgba(255, 0, 0, 0.1); color: var(--youtube); border-color: var(--youtube); }
        .youtube-btn:hover { background: var(--youtube); color: white; box-shadow: 0 0 20px rgba(255, 0, 0, 0.5); transform: translateY(-3px); }

        .discord-btn { background: rgba(88, 101, 242, 0.1); color: var(--discord); border-color: var(--discord); }
        .discord-btn:hover { background: var(--discord); color: white; box-shadow: 0 0 20px rgba(88, 101, 242, 0.5); transform: translateY(-3px); }

        /* --- Expertise --- */
        .section { padding: 100px 8%; text-align: center; }
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; margin-top: 50px; }

        .card {
            background: var(--card-bg); padding: 50px 30px; border-radius: 24px;
            border: 1px solid #1f1f1f; transition: 0.4s; position: relative;
        }
        .card:hover { transform: translateY(-10px); border-color: var(--rrx-red); }
        .card-gear { position: absolute; top: -10px; left: -10px; font-size: 2.5rem; color: rgba(255, 49, 49, 0.15); }
        .card:hover .card-gear { color: var(--rrx-red); animation: rotate 5s infinite linear; }
        .card h3 { color: #fff; margin-bottom: 15px; font-family: 'Orbitron'; }

        /* --- Contact Section --- */
        .contact-section { background: #050505; border-top: 1px solid #111; padding: 100px 8%; text-align: center; }
        .contact-card { 
            background: linear-gradient(145deg, #0f0f0f, #151515); 
            padding: 50px 30px; border-radius: 25px; 
            display: inline-block; width: 100%; max-width: 700px; 
            border: 1px solid #222;
        }
        .contact-card a { color: var(--rrx-red); text-decoration: none; font-size: clamp(1rem, 5vw, 1.8rem); font-weight: 800; transition: 0.3s; word-break: break-all; }

        /* --- Footer --- */
        footer { padding: 80px 8% 40px; background: #000; text-align: center; border-top: 1px solid #111; }
        .footer-link-box { margin-bottom: 30px; }
        .premium-link { padding: 10px 30px; border: 1px solid var(--rrx-red); color: var(--rrx-red); text-decoration: none; border-radius: 30px; font-size: 0.8rem; font-weight: 600; transition: 0.3s; }
        .premium-link:hover { background: var(--rrx-red); color: #000; box-shadow: 0 0 15px var(--rrx-red); }

        .copyright {
            color: rgba(255, 49, 49, 0.9); font-size: 0.75rem; letter-spacing: 1px; margin-top: 40px;
            text-transform: uppercase; font-family: 'Rajdhani';
            text-shadow: 0 0 10px var(--rrx-red), 0 0 5px var(--rrx-red); /* Glowing Effect */
        }

        @media (max-width: 600px) {
            nav { padding: 0 15px; }
            .logo { font-size: 1rem; margin-right: 15px; }
            .nav-links { gap: 10px; }
        }
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
        <div class="hero-gear hero-gear-1">⚙️</div>
        <div class="hero-gear hero-gear-2">⚙️</div>
        <h1 class="glitch-title">RRX STUDIOS</h1>
        <p>Innovation in Motion</p>
        
        <div class="social-group">
            <a href="http://www.youtube.com/@RRXSTUDIOS" target="_blank" class="btn-social youtube-btn">YouTube</a>
            <a href="https://discord.gg/vGKpaZdFtt" target="_blank" class="btn-social discord-btn">Discord</a>
        </div>
    </section>

    <section id="expertise" class="section">
        <h2 style="font-family: 'Orbitron'; letter-spacing: 5px; color: var(--rrx-red);">OUR EXPERTISE</h2>
        <div class="grid">
            <div class="card">
                <div class="card-gear">⚙️</div>
                <h3>Digital Content</h3>
                <p style="color: #888;">High-fidelity video production and immersive storytelling.</p>
            </div>
            <div class="card">
                <div class="card-gear">⚙️</div>
                <h3>Innovation</h3>
                <p style="color: #888;">Designing next-gen digital ecosystems via technology.</p>
            </div>
            <div class="card">
                <div class="card-gear">⚙️</div>
                <h3>Brand Identity</h3>
                <p style="color: #888;">Unique visual legacies that dominate the industry.</p>
            </div>
        </div>
    </section>

    <section id="contact" class="contact-section">
        <h2 style="font-family: 'Orbitron'; letter-spacing: 5px; color: var(--rrx-red); margin-bottom: 40px;">GET IN TOUCH</h2>
        <div class="contact-card">
            <p style="color: #666; margin-bottom: 15px; font-weight: 600; text-transform: uppercase;">Support Mail</p>
            <a href="mailto:rrxstudiosofficial@gmail.com">rrxstudiosofficial@gmail.com</a>
        </div>
    </section>

    <footer>
        <div class="footer-link-box">
            <a href="https://rrxstudios.github.io/RRXCORE/" target="_blank" class="premium-link">RRX CORE</a>
        </div>
        <p style="color: var(--rrx-red); font-weight: 700; letter-spacing: 2px; text-transform: uppercase; font-size: 0.8rem;">RRX Network</p>
        <p class="copyright">&copy; 2026 RRX STUDIOS | POWERED BY REDRROX</p>
    </footer>

</body>
</html>
