<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RRX STUDIOS</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #0b0c10;
            color: #c5c6c7;
            scroll-behavior: smooth;
        }

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 50px;
            background-color: #1f2833;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        header .logo {
            font-size: 1.8em;
            font-weight: bold;
            color: #66fcf1;
        }

        nav a {
            color: #45a29e;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #66fcf1;
        }

        .hero {
            height: 90vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: linear-gradient(rgba(11, 12, 16, 0.8), rgba(11, 12, 16, 0.8)), url('https://via.placeholder.com/1920x1080'); /* Replace with a real background if available */
            background-size: cover;
            background-position: center;
        }

        .hero h1 {
            font-size: 4em;
            color: #66fcf1;
            margin: 0;
        }

        .hero p {
            font-size: 1.5em;
            margin: 20px 0;
        }

        .cta-buttons {
            display: flex;
            gap: 30px;
            margin-top: 20px;
        }

        .cta-buttons a i {
            font-size: 45px;
            transition: transform 0.3s, color 0.3s;
            color: #66fcf1;
        }

        .cta-buttons a:hover i {
            transform: scale(1.2);
        }

        .fa-youtube:hover {
            color: #FF0000;
        }

        .fa-discord:hover {
            color: #5865F2;
        }

        .expertise {
            padding: 100px 50px;
            text-align: center;
        }

        .expertise h2 {
            font-size: 2.5em;
            color: #66fcf1;
            margin-bottom: 50px;
        }

        .expertise-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .card {
            background-color: #1f2833;
            padding: 40px;
            border-radius: 10px;
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-10px);
            border: 1px solid #66fcf1;
        }

        .card h3 {
            color: #66fcf1;
            margin-bottom: 15px;
        }

        .contact {
            padding: 100px 50px;
            background-color: #1f2833;
            text-align: center;
        }

        .contact h2 {
            color: #66fcf1;
            margin-bottom: 20px;
        }

        .contact a {
            color: #66fcf1;
            text-decoration: none;
            font-size: 1.2em;
        }

        footer {
            padding: 30px;
            text-align: center;
            background-color: #0b0c10;
            border-top: 1px solid #1f2833;
        }

        .footer-links a {
            color: #45a29e;
            text-decoration: none;
            margin: 0 10px;
            font-size: 0.9em;
        }

        @media (max-width: 768px) {
            header {
                flex-direction: column;
                padding: 20px;
            }
            .hero h1 {
                font-size: 2.5em;
            }
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
    <div class="icon-gear">⚙️</div>
    <div class="icon-gear-small">⚙️</div>
    <h1>RRX STUDIOS</h1>
    <p>Innovation in Motion</p>
    <div class="cta-buttons">
        <a href="http://www.youtube.com/@RRXSTUDIOS" target="_blank" title="YouTube">
            <i class="fa-brands fa-youtube"></i>
        </a>
        <a href="https://discord.gg/vGKpaZdFtt" target="_blank" title="Discord">
            <i class="fa-brands fa-discord"></i>
        </a>
    </div>
</section>

<section id="expertise" class="expertise">
    <h2>OUR EXPERTISE</h2>
    <div class="expertise-grid">
        <div class="card">
            <div class="icon">⚙️</div>
            <h3>Digital Content</h3>
            <p>High-fidelity video production and immersive storytelling.</p>
        </div>
        <div class="card">
            <div class="icon">⚙️</div>
            <h3>Innovation</h3>
            <p>Designing next-gen digital ecosystems via technology.</p>
        </div>
        <div class="card">
            <div class="icon">⚙️</div>
            <h3>Brand Identity</h3>
            <p>Unique visual legacies that dominate the industry.</p>
        </div>
    </div>
</section>

<section id="contact" class="contact">
    <h2>GET IN TOUCH</h2>
    <p>Support Mail</p>
    <a href="mailto:rrxstudiosofficial@gmail.com">rrxstudiosofficial@gmail.com</a>
</section>

<footer>
    <div class="footer-links">
        <a href="https://rrxstudios.github.io/RRXCORE/">RRX CORE</a>
        <a href="#">RRX Network</a>
    </div>
    <p>&copy; 2026 RRX Studios | Powered by RedRrox</p>
</footer>

</body>
</html>
