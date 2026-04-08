<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RRX STUDIOS | Innovation in Motion</title>
    <style>
        :root {
            --primary-color: #FFD700; /* Gold/Yellow */
            --bg-dark: #0a0a0a;
            --text-light: #ffffff;
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--bg-dark);
            color: var(--text-light);
            overflow-x: hidden;
        }

        /* Navbar Styling */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 10%;
            background: rgba(0, 0, 0, 0.8);
            backdrop-filter: blur(10px);
            position: fixed;
            width: 80%;
            z-index: 1000;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--primary-color);
            letter-spacing: 2px;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: radial-gradient(circle, #1a1a1a 0%, #000000 100%);
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 5px;
            animation: fadeIn 2s ease-in;
        }

        .hero p {
            font-size: 1.2rem;
            color: #888;
            margin-bottom: 30px;
        }

        .cta-btn {
            padding: 15px 40px;
            background-color: var(--primary-color);
            color: #000;
            text-decoration: none;
            font-weight: bold;
            border-radius: 50px;
            transition: 0.3s;
            box-shadow: 0 0 20px rgba(255, 215, 0, 0.4);
        }

        .cta-btn:hover {
            transform: scale(1.1);
            box-shadow: 0 0 30px rgba(255, 215, 0, 0.7);
        }

        /* About Section */
        .about {
            padding: 100px 10%;
            text-align: center;
            background-color: #0f0f0f;
        }

        .about h2 {
            color: var(--primary-color);
            font-size: 2.5rem;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 50px;
        }

        .card {
            background: #1a1a1a;
            padding: 30px;
            border-radius: 15px;
            border-bottom: 3px solid var(--primary-color);
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-10px);
        }

        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">RRX STUDIOS</div>
        <div>
            </div>
    </nav>

    <section class="hero">
        <h1>RRX STUDIOS</h1>
        <p>Innovation in Motion | Digital Excellence</p>
        <a href="#about" class="cta-btn">Discover Our World</a>
    </section>

    <section id="about" class="about">
        <h2>Our Expertise</h2>
        <div class="grid">
            <div class="card">
                <h3>Digital Content</h3>
                <p>Creating immersive experiences through high-quality video production and gaming content.</p>
            </div>
            <div class="card">
                <h3>Innovation</h3>
                <p>Pushing the boundaries of tech and creativity to build future-ready solutions.</p>
            </div>
            <div class="card">
                <h3>Brand Identity</h3>
                <p>Developing unique identities that stand out in the crowded digital landscape.</p>
            </div>
        </div>
    </section>

</body>
</html>
