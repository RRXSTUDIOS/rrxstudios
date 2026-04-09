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
            --text-light: #ffffff;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: 'Rajdhani', sans-serif;
            background-color: var(--bg-dark);
            color: var(--text-light);
            overflow-x: hidden; /* স্ক্রিন ডানে সরবে না */
            width: 100%;
        }

        /* --- Navbar Fix (সব শুরুতে আনার জন্য) --- */
        nav {
            height: 75px;
            background: rgba(8, 2, 13, 0.98);
            backdrop-filter: blur(15px);
            position: fixed; top: 0; width: 100%; z-index: 10000;
            border-bottom: 2px solid var(--rrx-red);
            display: flex;
            align-items: center;
            padding: 0 20px; /* সাইড প্যাডিং */
        }

        .logo {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.2rem; font-weight: 900;
            color: white; letter-spacing: 1.5px;
            text-shadow: 2px 0 var(--rrx-red);
            margin-right: 40px; /* লোগো থেকে মেনুর দূরত্ব */
        }

        .nav-links { 
            display: flex; 
            gap: 20px; /* মেনুর মাঝখানের গ্যাপ */
        } 
        .nav-links a {
            color: #ccc; text-decoration: none;
            font-size: 0.85rem; font-weight: 700; text-transform: uppercase; transition: 0.3s;
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
            font-size: clamp(2.2rem, 10vw, 5.5rem);
            font-weight: 900; position: relative; color: white;
            text-transform: uppercase; letter-spacing: 5px;
            text-shadow: 0 0 15px var(--rrx-red); z-index: 1;
        }
        .title-gear { font-size: 1.5rem; color: var(--rrx-red); vertical-align: middle; margin: 0 10px; }

        /* --- Expertise --- */
        .section { padding: 100px 8%; text-align: center; }
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; margin-top: 50px; }

        .card {
            background: rgba(20, 20, 20, 0.7); padding: 50px 30px; border-radius: 24px;
            border: 1px solid #1f1f1f; transition: 0.4s; position: relative;
        }
        .card:hover { transform: translateY(-10px); border-color: var(--rrx-red); }
        .card-gear { position: absolute; top: -10px; left: -10px; font-size: 2.5rem; color: rgba(255, 49, 49, 0.15); }
        .card:hover .card-gear { color: var(--rrx-red); animation: rotate 5s infinite linear; }

        /* --- Contact --- */
        .contact-section { background: #050505; border-top: 1px solid #111; padding: 80px 8%; text-align: center; }
        .contact-card { 
            background: linear-gradient(145deg, #0f0f0f, #151515); 
            padding: 40px 20px; border-radius: 20px; 
            border: 1px solid #222; width: 100%; max-width: 600px; display: inline-block;
        }
        .contact-card a { color: var(--rrx-red); text-decoration: none; font-size: clamp(0.9rem, 4vw, 1.5rem); font-weight: 800; word-break: break-all; }

        /* --- Footer --- */
        footer { padding: 40px; background: #000; text-align: center; border-top: 1px solid #111; }
        .copyright {
            color: rgba(255, 49, 49, 0.9); font-size: 0.75rem; letter-spacing: 1px; margin-top: 20px;
            text-shadow: 0 0 10px var(--rrx-red);
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
        <h1 class="glitch-title"><span class="title-gear">⚙️</span>RRX STUDIOS<span class="title-gear">⚙️</span></h1>
        <p style="font-family: 'Orbitron'; letter-spacing: 4px; color: #888; margin-top: 10px;">Innovation in Motion</p>
    </section>

    <section id="expertise" class="section">
        <h2 style="font-family: 'Orbitron'; letter-spacing: 5px; color: var(--rrx-red);">OUR EXPERTISE</h2>
        <div class="grid">
            <div class="card">
                <div class="card-gear">⚙️</div>
                <h3 style="color: #fff; margin-bottom: 15px; font-family: 'Orbitron';">Digital Content</h3>
                <p style="color: #888;">High-fidelity video production and immersive storytelling.</p>
            </div>
            <div class="card">
                <div class="card-gear">⚙️</div>
                <h3 style="color: #fff; margin-bottom: 15px; font-family: 'Orbitron';">Innovation</h3>
                <p style="color: #888;">Designing next-gen digital ecosystems via tech.</p>
            </div>
        </div>
    </section>

    <section id="contact" class="contact-section">
        <div class="contact-card">
            <p style="color: #666; margin-bottom: 10px; font-size: 0.8rem; letter-spacing: 2px;">OFFICIAL SUPPORT</p>
            <a href="mailto:rrxstudiosofficial@gmail.com">rrxstudiosofficial@gmail.com</a>
        </div>
    </section>

    <footer>
        <p class="copyright">&copy; 2026 RRX STUDIOS | POWERED BY REDRROX</p>
    </footer>

</body>
</html>
