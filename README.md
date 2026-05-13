<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RRX STUDIOS | Powered by RedRrox</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    
    <style>
        :root {
            /* লোগোর কালার অনুযায়ী পার্পল এবং রেড সেট করা হয়েছে */
            --bg-deep: #0d0216; 
            --purple-glow: #1a0533;
            --accent-red: #ff003c;
            --neon-glow: 0 0 15px #ff003c, 0 0 30px #ff003c;
            --text-color: #ffffff;
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Poppins', sans-serif;
            /* লোগোর ব্যাকগ্রাউন্ডের মতো ডার্ক পার্পল গ্রেডিয়েন্ট */
            background: radial-gradient(circle at center, #1a0533 0%, #05010a 100%);
            color: var(--text-color);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        /* --- Animations --- */
        @keyframes rotateGear {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        @keyframes pulseRed {
            0% { text-shadow: 0 0 10px var(--accent-red); }
            50% { text-shadow: 0 0 30px var(--accent-red), 0 0 50px var(--accent-red); }
            100% { text-shadow: 0 0 10px var(--accent-red); }
        }

        /* --- Header (Clean & No Extra Text) --- */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 60px;
            background-color: rgba(5, 1, 10, 0.95);
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 2px solid var(--accent-red);
            box-shadow: 0 0 20px rgba(255, 0, 60, 0.4);
        }

        header .logo {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.8em;
            font-weight: bold;
            color: #fff;
            text-shadow: var(--neon-glow);
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
            text-shadow: var(--neon-glow);
        }

        /* --- Hero Section --- */
        .hero {
            height: 85vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 20px;
        }

        .gear-main {
            font-size: 120px;
            color: var(--accent-red);
            margin-bottom: 30px;
            animation: rotateGear 5s linear infinite;
            filter: drop-shadow(var(--neon-glow));
        }

        .hero h1 {
            font-family: 'Orbitron', sans-serif;
            font-size: 5em;
            color: #fff;
            margin: 0;
            text-shadow: var(--neon-glow);
            animation: pulseRed 2s infinite ease-in-out;
            letter-spacing: 2px;
        }

        .hero p {
            font-size: 1.4em;
            margin: 15px 0;
            letter-spacing: 8px;
            text-transform: uppercase;
            opacity: 0.9;
        }

        /* --- Icons Only --- */
        .social-container {
            display: flex;
            gap: 45px;
            margin-top: 40px;
        }

        .social-container a i {
            font-size: 60px;
            color: #fff;
            transition: 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        .fa-youtube:hover {
            color: #ff0000;
            filter: drop-shadow(0 0 15px #ff0000);
            transform: scale(1.3);
        }

        .fa-discord:hover {
            color: #5865F2;
            filter: drop-shadow(0 0 15px #5865F2);
            transform: scale(1.3);
        }

        /* --- Expertise --- */
        .expertise {
            padding: 100px 60px;
            text-align: center;
        }

        .expertise h2 {
            font-family: 'Orbitron', sans-serif;
            font-size: 3em;
            color: #fff;
            text-shadow: var(--neon-glow);
            margin-bottom: 60px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }

        .card {
            background: rgba(26, 5, 51, 0.6);
            padding: 50px;
            border-radius: 20px;
            border: 1px solid rgba(255, 0, 60, 0.2);
            backdrop-filter: blur(10px);
            transition: 0.4s;
        }

        .card:hover {
            transform: translateY(-15px);
            border: 1px solid var(--accent-red);
            box-shadow: 0 0 30px rgba(255, 0, 60, 0.4);
            background: rgba(26, 5, 51, 0.8);
        }

        .card i {
            font-size: 50px;
            color: var(--accent-red);
            margin-bottom: 25px;
            animation: rotateGear 10s linear infinite;
        }

        /* --- Contact --- */
        .contact {
            padding: 100px 60px;
            background: rgba(5, 1, 10, 0.9);
            text-align: center;
            border-top: 2px solid var(--accent-red);
        }

        .contact a {
            color: var(--accent-red);
            text-decoration: none;
            font-size: 1.8em;
            font-weight: bold;
            text-shadow: 0 0 10px var(--accent-red);
        }

        footer {
            padding: 50px;
            text-align: center;
            background: #000;
        }

        footer p {
            color: #fff;
            text-shadow: 0 0 5px var(--accent-red);
        }

        /* Mobile View Fix */
        @media (max-width: 768px) {
            .hero h1 { font-size: 3em; }
            header { padding: 20px; }
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
    <div class="gear-main">
        <i class="fa-solid fa-gear"></i>
    </div>
    <h1>RRX STUDIOS</h1>
    <p>Innovation in Motion</p>
    
    <div class="social-container">
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
    <div class="grid">
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
    <p>&copy; 2026 RRX STUDIOS | POWERED BY REDRROX</p>
</footer>

</body>
</html>
