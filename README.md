<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RRX STUDIOS | Powered by RedRrox</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    
    <style>
        :root {
            /* লোগোর কালার প্যালেট অনুযায়ী পার্পল এবং রেড সেট করা হয়েছে */
            --bg-color: #1a0b2e; 
            --secondary-bg: rgba(31, 40, 51, 0.8);
            --accent-red: #ff003c;
            --glow-shadow: 0 0 15px #ff003c, 0 0 30px #ff003c;
            --text-color: #e0e0e0;
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Poppins', sans-serif;
            /* লোগোর ব্যাকগ্রাউন্ডের মতো পার্পল গ্রেডিয়েন্ট এবং ডট ইফেক্ট */
            background: radial-gradient(circle, #2e1a47 0%, #0b051a 100%);
            background-image: radial-gradient(rgba(255, 255, 255, 0.05) 1px, transparent 1px);
            background-size: 20px 20px; /* ডট টেক্সচার */
            color: var(--text-color);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        /* --- Animations --- */
        @keyframes rotateGear {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        @keyframes pulseGlow {
            0% { text-shadow: 0 0 10px var(--accent-red); }
            50% { text-shadow: 0 0 30px var(--accent-red), 0 0 50px var(--accent-red); }
            100% { text-shadow: 0 0 10px var(--accent-red); }
        }

        /* --- Header --- */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 50px;
            background-color: rgba(11, 5, 26, 0.9);
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 2px solid var(--accent-red);
            box-shadow: 0 0 20px rgba(255, 0, 60, 0.3);
        }

        header .logo {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.8em;
            font-weight: bold;
            color: #fff;
            text-shadow: var(--glow-shadow);
        }

        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
            text-transform: uppercase;
            transition: 0.3s;
        }

        nav a:hover {
            color: var(--accent-red);
            text-shadow: var(--glow-shadow);
        }

        /* --- Hero Section --- */
        .hero {
            height: 85vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        .gear-container {
            font-size: 110px;
            color: var(--accent-red);
            margin-bottom: 25px;
            animation: rotateGear 6s linear infinite;
            filter: drop-shadow(var(--glow-shadow));
        }

        .hero h1 {
            font-family: 'Orbitron', sans-serif;
            font-size: 4.5em;
            color: #fff;
            margin: 0;
            text-shadow: var(--glow-shadow);
            animation: pulseGlow 2.5s infinite ease-in-out;
        }

        .hero p {
            font-size: 1.3em;
            margin: 10px 0;
            letter-spacing: 6px;
            text-transform: uppercase;
            color: #fff;
            opacity: 0.9;
        }

        /* --- Social Icons Only --- */
        .cta-buttons {
            display: flex;
            gap: 40px;
            margin-top: 35px;
        }

        .cta-buttons a i {
            font-size: 55px;
            color: #fff;
            transition: 0.4s;
        }

        .cta-buttons a .fa-youtube:hover {
            color: #ff0000;
            filter: drop-shadow(0 0 15px #ff0000);
            transform: scale(1.2) rotate(5deg);
        }

        .cta-buttons a .fa-discord:hover {
            color: #5865F2;
            filter: drop-shadow(0 0 15px #5865F2);
            transform: scale(1.2) rotate(-5deg);
        }

        /* --- Expertise Section --- */
        .expertise {
            padding: 80px 50px;
            text-align: center;
        }

        .expertise h2 {
            font-family: 'Orbitron', sans-serif;
            font-size: 2.8em;
            color: #fff;
            text-shadow: var(--glow-shadow);
            margin-bottom: 50px;
        }

        .expertise-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 35px;
        }

        .card {
            background-color: rgba(31, 40, 51, 0.4);
            padding: 45px;
            border-radius: 20px;
            border: 1px solid rgba(255, 0, 60, 0.2);
            backdrop-filter: blur(5px);
            transition: 0.4s;
        }

        .card:hover {
            transform: translateY(-12px);
            border: 1px solid var(--accent-red);
            box-shadow: 0 0 25px rgba(255, 0, 60, 0.4);
            background-color: rgba(31, 40, 51, 0.6);
        }

        .card i {
            font-size: 45px;
            color: var(--accent-red);
            margin-bottom: 25px;
            animation: rotateGear 12s linear infinite;
        }

        .card h3 {
            font-family: 'Orbitron', sans-serif;
            color: #fff;
            margin-bottom: 15px;
        }

        /* --- Contact --- */
        .contact {
            padding: 90px 50px;
            background-color: rgba(11, 5, 26, 0.8);
            text-align: center;
            border-top: 2px solid var(--accent-red);
        }

        .contact a {
            color: var(--accent-red);
            text-decoration: none;
            font-size: 1.6em;
            font-weight: bold;
            text-shadow: 0 0 8px var(--accent-red);
            transition: 0.3s;
        }

        .contact a:hover {
            letter-spacing: 1px;
        }

        /* --- Footer --- */
        footer {
            padding: 50px;
            text-align: center;
            background-color: #05020a;
        }

        footer p {
            font-size: 1em;
            color: #fff;
            text-shadow: 0 0 5px var(--accent-red);
        }

        .footer-links a {
            color: #aaa;
            text-decoration: none;
            margin: 0 15px;
            transition: 0.3s;
        }

        .footer-links a:hover {
            color: var(--accent-red);
        }

        @media (max-width: 768px) {
            .hero h1 { font-size: 2.8em; }
            header { padding: 15px 25px; }
            nav { display: none; }
        }
    </style>
</head>
<body>

<header>
    <div class="logo">RRX STUDIOS</div>
    <nav>
        <a href="#">Home</a>
        <a href="#expertise">Expertise</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="hero">
    <div class="gear-container">
        <i class="fa-solid fa-gear"></i>
    </div>
    <h1>RRX STUDIOS</h1>
    <p>Innovation in Motion</p>
    
    <div class="cta-buttons">
        <a href="http://www.youtube.com/@RRXSTUDIOS" target="_blank">
            <i class="fa-brands fa-youtube"></i>
        </a>
        <a href="https://discord.gg/vGKpaZdFtt" target="_blank">
            <i class="fa-brands fa-discord"></i>
        </a>
    </div>
</section>

<section id="expertise" class="expertise">
    <h2>OUR EXPERTISE</h2>
    <div class="expertise-grid">
        <div class="card">
            <i class="fa-solid fa-cog"></i>
            <h3>Digital Content</h3>
            <p>High-fidelity video production and immersive storytelling.</p>
        </div>
        <div class="card">
            <i class="fa-solid fa-cog"></i>
            <h3>Innovation</h3>
            <p>Designing next-gen digital ecosystems via technology.</p>
        </div>
        <div class="card">
            <i class="fa-solid fa-cog"></i>
            <h3>Brand Identity</h3>
            <p>Unique visual legacies that dominate the industry.</p>
        </div>
    </div>
</section>

<section id="contact" class="contact">
    <h2>GET IN TOUCH</h2>
    <p>Official Support Mail</p>
    <a href="mailto:rrxstudiosofficial@gmail.com">rrxstudiosofficial@gmail.com</a>
</section>

<footer>
    <div class="footer-links" style="margin-bottom: 20px;">
        <a href="https://rrxstudios.github.io/RRXCORE/">RRX CORE</a>
        <a href="#">RRX Network</a>
    </div>
    <p>&copy; 2026 RRX STUDIOS | POWERED BY REDRROX</p>
</footer>

</body>
</html>
