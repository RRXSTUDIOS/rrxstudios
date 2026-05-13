<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RRX STUDIOS | Powered by RedRrox</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    
    <style>
        /* CSS Variables for Easy Theme Control */
        :root {
            --bg-color: #0b0c10;
            --secondary-bg: #1f2833;
            --accent-red: #ff003c;
            --glow-shadow: 0 0 10px #ff003c, 0 0 20px #ff003c, 0 0 30px #ff003c;
            --text-color: #c5c6c7;
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Poppins', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        /* --- Animations --- */
        @keyframes slideInUp {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes rotateGear {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        @keyframes pulseGlow {
            0% { text-shadow: 0 0 10px var(--accent-red); }
            50% { text-shadow: 0 0 25px var(--accent-red), 0 0 40px var(--accent-red); }
            100% { text-shadow: 0 0 10px var(--accent-red); }
        }

        /* --- Header --- */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 50px;
            background-color: var(--secondary-bg);
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 2px solid var(--accent-red);
            box-shadow: 0 5px 15px rgba(255, 0, 60, 0.2);
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
            height: 90vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: radial-gradient(circle, rgba(108, 44, 245, 0.05) 0%, rgba(11, 12, 16, 1) 80%);
        }

        .gear-container {
            font-size: 100px;
            color: var(--accent-red);
            margin-bottom: 20px;
            animation: rotateGear 5s linear infinite;
            filter: drop-shadow(var(--glow-shadow));
        }

        .hero h1 {
            font-family: 'Orbitron', sans-serif;
            font-size: 5em;
            color: #fff;
            margin: 0;
            text-shadow: var(--glow-shadow);
            animation: pulseGlow 2s infinite ease-in-out;
        }

        .hero p {
            font-size: 1.5em;
            margin: 10px 0;
            letter-spacing: 5px;
            text-transform: uppercase;
        }

        /* --- Only Social Icons --- */
        .cta-buttons {
            display: flex;
            gap: 40px;
            margin-top: 30px;
        }

        .cta-buttons a {
            text-decoration: none;
            transition: 0.3s;
        }

        .cta-buttons a i {
            font-size: 50px;
            color: #fff;
            transition: 0.3s;
        }

        .cta-buttons a .fa-youtube:hover {
            color: #ff0000;
            filter: drop-shadow(0 0 10px #ff0000);
            transform: scale(1.2);
        }

        .cta-buttons a .fa-discord:hover {
            color: #5865F2;
            filter: drop-shadow(0 0 10px #5865F2);
            transform: scale(1.2);
        }

        /* --- Expertise Section --- */
        .expertise {
            padding: 100px 50px;
            text-align: center;
            animation: slideInUp 1s ease-out;
        }

        .expertise h2 {
            font-family: 'Orbitron', sans-serif;
            font-size: 3em;
            color: #fff;
            text-shadow: var(--glow-shadow);
            margin-bottom: 50px;
        }

        .expertise-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .card {
            background-color: var(--secondary-bg);
            padding: 40px;
            border-radius: 15px;
            border: 1px solid rgba(255, 0, 60, 0.1);
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-10px);
            border: 1px solid var(--accent-red);
            box-shadow: 0 0 20px rgba(255, 0, 60, 0.3);
        }

        .card i {
            font-size: 40px;
            color: var(--accent-red);
            margin-bottom: 20px;
            animation: rotateGear 10s linear infinite;
        }

        .card h3 {
            font-family: 'Orbitron', sans-serif;
            color: #fff;
            text-shadow: 0 0 5px var(--accent-red);
        }

        /* --- Contact --- */
        .contact {
            padding: 100px 50px;
            background-color: var(--secondary-bg);
            text-align: center;
            border-top: 2px solid var(--accent-red);
        }

        .contact h2 {
            font-family: 'Orbitron', sans-serif;
            color: #fff;
            text-shadow: var(--glow-shadow);
        }

        .contact a {
            color: var(--accent-red);
            text-decoration: none;
            font-size: 1.5em;
            font-weight: bold;
            text-shadow: 0 0 5px var(--accent-red);
        }

        /* --- Footer --- */
        footer {
            padding: 40px;
            text-align: center;
            background-color: var(--bg-color);
            border-top: 1px solid var(--secondary-bg);
        }

        footer p {
            font-size: 1.1em;
            color: #fff;
            text-shadow: 0 0 5px var(--accent-red);
        }

        .footer-links a {
            color: var(--text-color);
            text-decoration: none;
            margin: 0 15px;
            transition: 0.3s;
        }

        .footer-links a:hover {
            color: var(--accent-red);
        }

        /* --- Responsive --- */
        @media (max-width: 768px) {
            .hero h1 { font-size: 3em; }
            header { padding: 15px 20px; }
            nav { display: none; } /* Hide nav on mobile for clean look */
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
            <p>High-fidelity video production and immersive storytelling for the next gen.</p>
        </div>
        <div class="card">
            <i class="fa-solid fa-cog"></i>
            <h3>Innovation</h3>
            <p>Pushing the limits of technology to create unique digital ecosystems.</p>
        </div>
        <div class="card">
            <i class="fa-solid fa-cog"></i>
            <h3>Brand Identity</h3>
            <p>Crafting visual legacies that dominate the gaming and tech industry.</p>
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
