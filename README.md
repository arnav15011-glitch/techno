<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Arnav | Digital Services</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
    <link href="https://unpkg.com/aos@2.3.4/dist/aos.css" rel="stylesheet">

    <style>
        html { scroll-behavior: smooth; }
        body {
            margin: 0;
            font-family: 'Inter', sans-serif;
            background: #0f172a;
            color: white;
            line-height: 1.6;
        }
        header {
            padding: 20px 10%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: #0b1220;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        header h1 { color: #38bdf8; margin: 0; }
        header nav a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
            font-weight: bold;
            transition: 0.3s;
        }
        header nav a:hover { color: #38bdf8; }

        .hero { padding: 100px 10%; text-align: center; }
        .hero h2 { font-size: 2.8rem; margin-bottom: 20px; }
        .hero p { font-size: 1.2rem; color: #cbd5e1; margin-bottom: 30px; }

        .btn {
            background: #38bdf8;
            color: black;
            padding: 12px 25px;
            border-radius: 6px;
            text-decoration: none;
            font-weight: bold;
        }

        .section { padding: 70px 10%; text-align: center; }
        .dark { background: #1e293b; }

        .service-boxes, .pricing-boxes {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }

        .box {
            background: #0f172a;
            padding: 25px;
            border-radius: 8px;
            border: 1px solid #1e293b;
            transition: 0.3s;
        }
        .box:hover {
            transform: translateY(-6px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.3);
        }

        .box h4 { color: #38bdf8; }
        .box p { text-align: left; margin: 8px 0; }
        .box i { color: #22c55e; margin-right: 8px; }

        .price {
            font-size: 1.8rem;
            margin: 15px 0;
            color: #22c55e;
            font-weight: bold;
        }

        .qr-box img {
            width: 220px;
            max-width: 80%;
            border-radius: 12px;
            margin: 20px 0;
            border: 2px solid #1e293b;
        }

        .pay-btn {
            display: inline-block;
            margin-top: 10px;
            background: linear-gradient(45deg, #22c55e, #16a34a);
            color: white;
            padding: 12px 28px;
            border-radius: 8px;
            font-weight: bold;
            text-decoration: none;
            box-shadow: 0 0 15px rgba(34,197,94,0.6);
        }

        .utr-form {
            margin-top: 40px;
            background: #0f172a;
            padding: 25px;
            border-radius: 10px;
            border: 1px solid #1e293b;
        }

        .utr-form h4 { color: #38bdf8; }

        .utr-form input {
            width: 100%;
            padding: 12px;
            margin: 8px 0;
            border-radius: 6px;
            border: none;
            background: #1e293b;
            color: white;
        }

        .utr-form button {
            width: 100%;
            padding: 12px;
            background: #38bdf8;
            border: none;
            border-radius: 6px;
            font-weight: bold;
            cursor: pointer;
            margin-top: 10px;
        }

        footer {
            text-align: center;
            padding: 20px;
            background: #0b1220;
            color: #94a3b8;
        }
    </style>
</head>
<body>

<header>
    <h1>Arnav</h1>
    <nav>
        <a href="#services">Services</a>
        <a href="#pricing">Pricing</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="hero" data-aos="fade-up">
    <h2>I Build Clean & Modern Websites</h2>
    <p>Affordable websites for individuals and small businesses.</p>
    <a href="#contact" class="btn">Get Started</a>
</section>

<section id="services" class="section dark" data-aos="fade-up">
    <h3>My Services</h3>
    <div class="service-boxes">
        <div class="box"><h4>Website Design</h4><p>Modern and responsive layouts</p></div>
        <div class="box"><h4>Frontend Development</h4><p>Fast & clean websites</p></div>
        <div class="box"><h4>SEO Optimization</h4><p>Better Google ranking</p></div>
    </div>
</section>

<section id="pricing" class="section" data-aos="fade-up">
    <h3>Pricing Plans</h3>
    <div class="pricing-boxes">
        <div class="box">
            <h4>Starter</h4>
            <div class="price">₹799</div>
            <p><i class="fa-solid fa-check"></i> 1-page website</p>
            <p><i class="fa-solid fa-check"></i> Mobile responsive</p>
        </div>
        <div class="box">
            <h4>Professional</h4>
            <div class="price">₹999</div>
            <p><i class="fa-solid fa-check"></i> Up to 3 pages</p>
            <p><i class="fa-solid fa-check"></i> Contact section</p>
        </div>
        <div class="box">
            <h4>Business</h4>
            <div class="price">₹1500</div>
            <p><i class="fa-solid fa-check"></i> Up to 5 pages</p>
            <p><i class="fa-solid fa-check"></i> Basic SEO</p>
        </div>
    </div>
</section>

<section id="contact" class="section dark" data-aos="zoom-in">
    <h3>Pay & Confirm</h3>
    <p>Scan QR or click Pay Now</p>

    <div class="qr-box">
        <img src="qr.png" alt="Payment QR">
    </div>

    <a href="upi://pay?pa=8532016515@fam&pn=Arnav&cu=INR" class="pay-btn">💳 Pay Now</a>

    <div class="utr-form">
        <h4>Payment Confirmation</h4>
        <p>Enter your UTR after payment</p>
        <form action="https://formsubmit.co/arnav15042011@gmail.com" method="POST">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="text" name="utr" placeholder="Enter UTR Number" required>
            <button type="submit">Submit Payment Details</button>
        </form>
    </div>

    <p style="margin-top:20px;">
        📧 arnav15042011@gmail.com<br>
        💬 WhatsApp: 8532016515
    </p>
</section>

<footer>
    © 2026 Arnav. All rights reserved.
</footer>

<script src="https://unpkg.com/aos@2.3.4/dist/aos.js"></script>
<script>AOS.init({ duration: 1000, once: true });</script>

</body>
</html>
