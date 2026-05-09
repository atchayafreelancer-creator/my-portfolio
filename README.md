<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Atchaya A | UI/UX & Growth</title>
    
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;700&display=swap" rel="stylesheet">

    <style>
        :root {
            --bg: #ffffff;
            --accent: #E5D9D0; /* Matches your blazer */
            --dark: #1a1a1a;
            --gray: #666666;
        }

        * { 
            margin: 0; padding: 0; box-sizing: border-box; 
            font-family: 'Plus Jakarta Sans', sans-serif; 
        }

        body { background: var(--bg); color: var(--dark); line-height: 1.6; }

        /* Smooth Scrolling */
        html { scroll-behavior: smooth; }

        /* Navigation */
        nav { 
            display: flex; justify-content: space-between; align-items: center; 
            padding: 30px 8%; position: fixed; width: 100%; top: 0; 
            background: rgba(255,255,255,0.8); backdrop-filter: blur(10px); z-index: 1000;
        }

        .logo { font-weight: 700; font-size: 1.2rem; letter-spacing: -0.5px; }
        .nav-links a { text-decoration: none; color: var(--dark); margin-left: 40px; font-weight: 500; font-size: 0.9rem; }

        /* Hero Section */
        .hero { 
            min-height: 100vh; display: flex; align-items: center; 
            padding: 100px 8% 0; gap: 80px; 
        }

        .hero-content { flex: 1; }
        .hero-image { flex: 1; position: relative; }
        
        .hero-image img { 
            width: 100%; max-width: 450px; border-radius: 24px; 
            box-shadow: 0 30px 60px rgba(0,0,0,0.1); 
        }

        .hero-content h1 { font-size: 4.5rem; line-height: 1; margin-bottom: 24px; font-weight: 700; }
        .hero-content p { font-size: 1.25rem; color: var(--gray); margin-bottom: 40px; max-width: 500px; }

        /* Services Section */
        .services { padding: 120px 8%; background: #fdfdfd; }
        .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; margin-top: 60px; }
        
        .card { 
            padding: 50px; border-radius: 24px; background: white; 
            border: 1px solid #eee; transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
        }

        .card:hover { transform: translateY(-10px); box-shadow: 0 20px 40px rgba(0,0,0,0.05); border-color: var(--accent); }
        .card h3 { margin-bottom: 15px; font-size: 1.5rem; }

        /* Portfolio */
        .portfolio { padding: 120px 8%; }
        .project-card { 
            height: 500px; background: var(--accent); border-radius: 30px; 
            margin-bottom: 40px; overflow: hidden; position: relative;
        }

        /* Buttons */
        .cta { 
            padding: 18px 40px; background: var(--dark); color: white; 
            text-decoration: none; border-radius: 100px; font-weight: 600; 
            display: inline-block; transition: 0.3s;
        }
        .cta:hover { transform: scale(1.05); background: #000; }

        @media (max-width: 900px) {
            .hero { flex-direction: column-reverse; text-align: center; padding-top: 150px; }
            .hero-content h1 { font-size: 3rem; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">ATCHAYA A.</div>
        <div class="nav-links">
            <a href="#services">Services</a>
            <a href="#work">Work</a>
            <a href="mailto:hello@atchaya.com" class="cta">Start a Project</a>
        </div>
    </nav>

    <section class="hero">
        <div class="hero-content" data-aos="fade-up">
            <h1 data-aos="fade-up" data-aos-delay="200">Scaling brands through <span style="color: var(--gray)">thoughtful design.</span></h1>
            <p data-aos="fade-up" data-aos-delay="400">Helping small businesses grow with premium UI/UX, high-converting E-commerce stores, and Meta Ad strategies.</p>
            <a href="#services" class="cta" data-aos="fade-up" data-aos-delay="600">Explore Services</a>
        </div>
        <div class="hero-image" data-aos="zoom-in" data-aos-delay="400">
            <img src="profile.jpg" alt="Atchaya A">
        </div>
    </section>

    <section id="services" class="services">
        <h2 style="font-size: 2.5rem;" data-aos="fade-right">My Expertise</h2>
        <div class="grid">
            <div class="card" data-aos="fade-up" data-aos-delay="100">
                <h3>UI/UX Design</h3>
                <p>User-centered interfaces that make your app or website easy to use and beautiful to look at.</p>
            </div>
            <div class="card" data-aos="fade-up" data-aos-delay="200">
                <h3>E-commerce</h3>
                <p>Building Shopify and Web stores designed to turn your visitors into loyal customers.</p>
            </div>
            <div class="card" data-aos="fade-up" data-aos-delay="300">
                <h3>Meta & Ads</h3>
                <p>Data-driven Instagram and Facebook ad campaigns that actually scale your revenue.</p>
            </div>
        </div>
    </section>

    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({
            duration: 1000,
            once: true,
            offset: 100
        });
    </script>
</body>
</html>
