<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gautam Banerjee - Insurance Broker</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #2563eb;
            --secondary: #0ea5e9;
            --accent: #f59e0b;
            --light: #f0f9ff;
            --dark: #1e3a8a;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f8fafc;
            color: #334155;
            line-height: 1.6;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 2rem 1rem;
            text-align: center;
        }
        
        .logo {
            font-size: 2.2rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }
        
        .tagline {
            font-size: 1.2rem;
            opacity: 0.9;
            margin-bottom: 1.5rem;
        }
        
        .contact-banner {
            background: rgba(255, 255, 255, 0.2);
            padding: 1rem;
            border-radius: 10px;
            display: inline-block;
            margin: 1rem 0;
        }
        
        .contact-banner a {
            color: white;
            text-decoration: none;
            font-size: 1.3rem;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 10px;
            justify-content: center;
        }
        
        .cta-button {
            display: inline-block;
            background-color: var(--accent);
            color: white;
            padding: 12px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            margin-top: 1rem;
            transition: all 0.3s ease;
        }
        
        .container {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 1rem;
        }
        
        .section {
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            padding: 2rem;
            margin-bottom: 2rem;
        }
        
        .section-title {
            color: var(--primary);
            border-bottom: 3px solid var(--secondary);
            padding-bottom: 0.5rem;
            margin-bottom: 1.5rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .about-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 2rem;
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }
        
        .service-card {
            background: #f0f9ff;
            border-radius: 10px;
            padding: 1.5rem;
            text-align: center;
            border-top: 4px solid var(--secondary);
        }
        
        .service-card i {
            font-size: 2.5rem;
            color: var(--secondary);
            margin-bottom: 1rem;
        }
        
        .timeline {
            position: relative;
            padding-left: 2rem;
        }
        
        .timeline::before {
            content: '';
            position: absolute;
            left: 7px;
            top: 0;
            height: 100%;
            width: 2px;
            background: var(--secondary);
        }
        
        .timeline-item {
            margin-bottom: 2rem;
            position: relative;
        }
        
        .timeline-item::before {
            content: '';
            position: absolute;
            left: -1.7rem;
            top: 8px;
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: var(--primary);
        }
        
        .contact-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 2rem;
        }
        
        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            margin-bottom: 1rem;
        }
        
        .contact-form button {
            background-color: var(--secondary);
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 5px;
            cursor: pointer;
            font-weight: 600;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 1rem;
        }
        
        footer {
            background: var(--dark);
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 2rem;
        }
        
        /* Image placeholders */
        .img-placeholder {
            height: 200px;
            background: linear-gradient(45deg, #dbeafe, #bfdbfe);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--primary);
            font-weight: 500;
            margin: 1rem 0;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <i class="fas fa-shield-alt"></i>
            <span>GAUTAM BANERJEE</span>
        </div>
        <div class="tagline">Expert Insurance Advisor | Auto & Home Insurance Specialist</div>
        <div class="contact-banner">
            <a href="tel:647-296-1087">
                <i class="fas fa-phone"></i> 647-296-1087
            </a>
        </div>
        <p>Over 9 years of experience providing tailored insurance solutions</p>
        <a href="#contact" class="cta-button">Get a Free Quote</a>
    </header>

    <div class="container">
        <section id="about" class="section">
            <h2 class="section-title"><i class="fas fa-user"></i> About Me</h2>
            <div class="about-grid">
                <p>RIBO Licensed insurance professional with 9+ years experience in Auto & Home insurance. I specialize in assessing client needs and providing optimal coverage solutions.</p>
                <p><strong>Trilingual:</strong> English, Hindi, Bengali</p>
                <div class="img-placeholder">Your Professional Photo</div>
            </div>
        </section>

        <section id="services" class="section">
            <h2 class="section-title"><i class="fas fa-handshake"></i> Services Offered</h2>
            <div class="services-grid">
                <div class="service-card">
                    <i class="fas fa-car"></i>
                    <h3>Auto Insurance</h3>
                    <p>Tailored coverage at excellent rates</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-home"></i>
                    <h3>Home Insurance</h3>
                    <p>Protect your most valuable asset</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-sync-alt"></i>
                    <h3>Policy Renewals</h3>
                    <p>Timely renewals with competitive rates</p>
                </div>
                <div class="service-card">
                    <i class="fas fa-user-friends"></i>
                    <h3>Client Advocacy</h3>
                    <p>Personalized support for claims</p>
                </div>
            </div>
        </section>

        <section id="testimonials" class="section">
            <h2 class="section-title"><i class="fas fa-comment"></i> Client Testimonials</h2>
            <div class="img-placeholder">BrokerLink President's Club Award</div>
            <p><i>"Your exceptional efforts have produced superior results. You are a BrokerLink top performer."</i></p>
            <p><strong>- Joe D'Annunzio, President</strong></p>
        </section>

        <section id="contact" class="section">
            <h2 class="section-title"><i class="fas fa-envelope"></i> Contact Me</h2>
            <div class="contact-grid">
                <div class="contact-form">
                    <form>
                        <input type="text" placeholder="Your Name" required>
                        <input type="email" placeholder="Your Email" required>
                        <input type="tel" placeholder="Your Phone">
                        <textarea placeholder="Your Message" rows="4" required></textarea>
                        <button type="submit">Send Message</button>
                    </form>
                </div>
                <div>
                    <div class="contact-item">
                        <i class="fas fa-phone"></i>
                        <div>
                            <h3>Phone</h3>
                            <p><a href="tel:647-296-1087">647-296-1087</a></p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-envelope"></i>
                        <div>
                            <h3>Email</h3>
                            <p><a href="mailto:g_banerjee@hotmail.com">g_banerjee@hotmail.com</a></p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-qrcode"></i>
                        <div>
                            <h3>Scan to Contact</h3>
                            <div class="img-placeholder" style="height: 150px;">QR Code</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <footer>
        <p>© 2024 Gautam Banerjee - Insurance Broker. All Rights Reserved.</p>
        <p>RIBO Licensed Since 2015</p>
    </footer>

    <script>
        // Simple form submission
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! I will contact you shortly.');
            this.reset();
        });
    </script>
</body>
</html>


