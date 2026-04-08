<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RRX STUDIOS | Innovation in Motion</title>
    <style>
        :root {
            --primary-color: #FFD700;
            --bg-dark: #0a0a0a;
            --card-bg: #141414;
            --text-light: #ffffff;
            --nav-height: 75px;
            --youtube: #FF0000;
            --discord: #5865F2;
        }

        * { box-sizing: border-box; }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Inter', 'Segoe UI', Roboto, sans-serif;
            background-color: var(--bg-dark);
            color: var(--text-light);
            scroll-behavior: smooth;
            overflow-x: hidden;
        }

        /* --- Navbar --- */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 8%;
            height: var(--nav-height);
            background: rgba(0, 0, 0, 0.9);
            backdrop-filter: blur(15px);
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 10000;
            border-bottom: 1px solid rgba(255, 215, 0, 0.05);
        }

        .logo {
            font-size: 1.4rem;
            font-weight: 900;
            color: var(--primary-color);
            letter-spacing: 3px;
            text-transform: uppercase;
        }

        .nav-links { display: flex; gap: 25px; }
        .nav-links a {
            color: #ccc;
            text-decoration: none;
            font-size: 0.85rem;
            font-weight: 600;
            text-transform: uppercase;
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
            padding: 20px;
            background: radial-gradient(circle at center, #111 0%, #000 100%);
        }

        .hero h1 {
            font-size: clamp(2.5rem, 10vw, 5.5rem);
            margin: 0;
            letter-spacing: 10px;
            font-weight: 900;
            background: linear-gradient(to bottom, #fff 40%, var(--primary-color));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero p {
            font-size: clamp(0.9rem, 4vw, 1.2rem);
            color: #666;
            margin-top: 10px;
            letter-spacing: 4px;
            text-transform: uppercase;
            margin-bottom: 30px;
        }

        /* --- Social Buttons --- */
        .social-group {
            display: flex;
            gap: 20px;
            margin-top: 10px;
            flex-wrap: wrap;
            justify-content: center;
        }

        .btn-social {
            padding: 12px 28px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 700;
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            display: flex;
            align-items: center;
            gap: 10px;
            border: 2px solid transparent;
        }

        .youtube-btn { background: rgba(255, 0, 0, 0.1); color: var(--youtube); border-color: var(--youtube); }
        .youtube-btn:hover { background: var(--youtube); color: white; box-shadow: 0 0 25px rgba(255, 0, 0, 0.5); transform: translateY(-5px); }

        .discord-btn { background: rgba(88, 101, 242, 0.1); color: var(--discord); border-color: var(--discord); }
        .discord-btn:hover { background: var(--discord); color: white; box-shadow: 0 0 25px rgba(88, 101, 242, 0.5); transform: translateY(-5px); }

        /* --- Expertise Section --- */
        .section { padding: 100px 8%; text-align: center; }
        .section-title { color: var(--primary-color); font-size: clamp(1.8rem, 5vw, 2.8rem); margin-bottom: 60px; font-weight: 800; text-transform: uppercase; }

        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; }

        .card { background: var(--card-bg); padding: 50px 30px; border-radius: 24px; border: 1px solid #1f1f1f; transition: all 0.5s cubic-bezier(0.2, 1, 0.3, 1); }
        .card:hover { transform: translateY(-15px); border-color: var(--primary-color); box-shadow: 0 20px 40px rgba(0, 0, 0, 0.6); }

        .card h3 { color: #fff; font-size: 1.6rem; margin-bottom: 20px; }
        .card p { color: #888; font-size: 1rem; line-height: 1.7; }

        /* --- Contact Section --- */
        .contact-section { background: #050505; border-top: 1px solid #111; }
        .contact-card { background: linear-gradient(145deg, #0f0f0f, #151515); padding: 60px 30px; border-radius: 30px; display: inline-block; width: 100%; max-width: 700px; border: 1px solid #222; }
        .contact-card a { color: var(--primary-color); text-decoration: none; font-size: clamp(1rem, 5vw, 1.8rem); font-weight: 800; transition: 0.3s; word-break: break-all; }

        /* --- Footer --- */
        footer { padding: 80px 8% 40px; background: #000; text-align: center; }
        .footer-nav-links { display: flex; justify-content: center; gap: 15px; flex-wrap: wrap; margin-top: 20px; }
        .premium-link-small { padding: 8px 20px; border: 1px solid var(--primary-color); color: var(--primary-color); text-decoration: none; border-radius: 30px; font-size: 0.75rem; font-weight: 600; transition: 0.3s; letter-spacing: 1px; }
        .premium-link-small:hover { background: var(--primary-color); color: #000; }

        .copyright { color: #333; font-size: 0.75rem; letter-spacing: 1px; margin-top: 40px; }

        @media (max-width: 768px) {
            nav { padding: 0 20px; justify-content: center; }
            .nav-links { display: none; }
            .section { padding: 80px 20px; }
            .hero h1 { letter-spacing: 5px; }
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
        <h1>RRX STUDIOS</h1>
        <p>Innovation in Motion</p>
        
        <div class="social-group">
            <a href="http://www.youtube.com/@RRXSTUDIOS" target="_blank" class="btn-social youtube-btn">YouTube</a>
            <a href="https://discord.gg/vGKpaZdFtt" target="_blank" class="btn-social discord-btn">Discord</a>
        </div>
    </section>

    <section id="expertise" class="section">
        <h2 class="section-title">Our Expertise</h2>
        <div class="grid">
            <div class="card">
                <h3>Digital Content</h3>
                <p>Creating immersive storytelling and high-fidelity video production for the digital era.</p>
            </div>
            <div class="card">
                <h3>Innovation</h3>
                <p>Designing and building next-gen digital ecosystems through cutting-edge technology.</p>
            </div>
            <div class="card">
                <h3>Brand Identity</h3>
                <p>Developing unique visual legacies that define and dominate the modern landscape.</p>
            </div>
        </div>
    </section>

    <section id="contact" class="section contact-section">
        <h2 class="section-title">Get In Touch</h2>
        <div class="contact-card">
            <p style="color: #666; margin-bottom: 20px; font-weight: 600; text-transform: uppercase; letter-spacing: 2px;">Support Mail</p>
            <a href="mailto:rrxstudiosofficial@gmail.com">rrxstudiosofficial@gmail.com</a>
        </div>
    </section>

    <footer>
        <p style="color: var(--primary-color); font-weight: 700; letter-spacing: 2px; text-transform: uppercase; font-size: 0.8rem;">RRX Network</p>
        <div class="footer-nav-links">
            <a href="https://rrxstudios.github.io/RRX/" target="_blank" class="premium-link-small">RRX CORE</a>
        </div>
        
        <p class="copyright">&copy; 2026 RRX STUDIOS | POWERED BY REDRROX</p>
    </footer>

</body>
</html>
