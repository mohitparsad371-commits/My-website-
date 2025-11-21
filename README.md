<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mohit Prasad Services</title>
  <meta name="google-site-verification" content="googleab29e5730f7fb514.html">
  
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background: linear-gradient(135deg, #0d1117 0%, #161b22 100%);
      color: #fff;
      line-height: 1.6;
      overflow-x: hidden;
      min-height: 100vh;
    }

    /* Header */
    header {
      background: rgba(0, 0, 0, 0.8);
      padding: 15px 0;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 1000;
      backdrop-filter: blur(5px);
      border-bottom: 1px solid rgba(0, 230, 118, 0.2);
    }

    .nav-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 20px;
    }

    .logo {
      font-size: 24px;
      font-weight: 700;
      color: #fff;
      text-decoration: none;
    }

    .logo span {
      color: #00e676;
    }

    .nav-menu {
      display: flex;
      list-style: none;
      gap: 20px;
    }

    .nav-menu a {
      color: #fff;
      text-decoration: none;
      font-size: 16px;
      font-weight: 500;
      transition: color 0.3s;
    }

    .nav-menu a:hover {
      color: #00e676;
    }

    .hamburger {
      display: none;
      cursor: pointer;
      font-size: 24px;
      color: #fff;
    }

    /* Hero Section */
    .hero {
      padding: 120px 20px 80px;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    .hero-content {
      max-width: 800px;
      margin: 0 auto;
      position: relative;
      z-index: 2;
    }

    .hero h1 {
      font-size: 2.5rem;
      margin-bottom: 20px;
      font-weight: 700;
      color: #fff;
      text-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
    }

    .hero p {
      font-size: 1.1rem;
      margin-bottom: 30px;
      color: rgba(255, 255, 255, 0.9);
    }

    .btn {
      display: inline-block;
      background: #00e676;
      color: #0d1117;
      padding: 12px 28px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      font-weight: 600;
      cursor: pointer;
      text-decoration: none;
      transition: all 0.3s;
      box-shadow: 0 4px 15px rgba(0, 200, 83, 0.3);
    }

    .btn:hover {
      background: #00a43a;
      transform: translateY(-3px);
      box-shadow: 0 6px 20px rgba(0, 200, 83, 0.4);
    }

    .btn-secondary {
      background: transparent;
      border: 2px solid #00e676;
      color: #00e676;
      margin-left: 15px;
    }

    .btn-secondary:hover {
      background: rgba(0, 230, 118, 0.1);
    }

    /* 3D Card Section */
    .section-title {
      text-align: center;
      margin-bottom: 40px;
      padding: 20px;
    }

    .section-title h2 {
      font-size: 2rem;
      color: #fff;
      margin-bottom: 15px;
      position: relative;
      display: inline-block;
    }

    .section-title h2:after {
      content: '';
      position: absolute;
      width: 70px;
      height: 3px;
      background: #00e676;
      bottom: -10px;
      left: 50%;
      transform: translateX(-50%);
    }

    .card-container {
      perspective: 1000px;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 25px;
      padding: 20px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .card {
      width: 300px;
      height: 380px;
      position: relative;
      transform-style: preserve-3d;
      transition: transform 0.5s ease;
      cursor: pointer;
    }

    .card-front, .card-back {
      position: absolute;
      width: 100%;
      height: 100%;
      backface-visibility: hidden;
      border-radius: 16px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 20px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    }

    .card-front {
      background: linear-gradient(145deg, #161b22, #1f2937);
      transform: rotateY(0deg);
    }

    .card-back {
      background: linear-gradient(145deg, #1f2937, #161b22);
      transform: rotateY(180deg);
      text-align: center;
    }

    .card.flipped {
      transform: rotateY(180deg);
    }

    .card-image {
      width: 100%;
      height: 160px;
      border-radius: 12px;
      overflow: hidden;
      margin-bottom: 20px;
    }

    .card-image img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.5s;
    }

    .card:hover .card-image img {
      transform: scale(1.05);
    }

    .card h3 {
      color: #00e676;
      font-size: 20px;
      margin-bottom: 10px;
      text-align: center;
    }

    .card p {
      text-align: center;
      margin-bottom: 15px;
      font-size: 14px;
    }

    .features {
      list-style: none;
      width: 100%;
    }

    .features li {
      padding: 6px 0;
      border-bottom: 1px solid rgba(255, 255, 255, 0.1);
      display: flex;
      align-items: center;
      font-size: 14px;
    }

    .features li:before {
      content: '✓';
      color: #00e676;
      margin-right: 10px;
      font-weight: bold;
    }

    /* Animated Background */
    .animated-bg {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: -1;
      overflow: hidden;
    }

    .bg-circle {
      position: absolute;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(0, 230, 118, 0.15) 0%, transparent 70%);
      opacity: 0.5;
      animation: float 15s infinite linear;
    }

    @keyframes float {
      0% {
        transform: translate(0, 0) scale(1);
        opacity: 0;
      }
      50% {
        opacity: 0.4;
      }
      100% {
        transform: translate(100px, -100px) scale(1.2);
        opacity: 0;
      }
    }

    /* Contact Section */
    .contact {
      padding: 60px 20px;
      text-align: center;
    }

    .contact-container {
      max-width: 800px;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 25px;
    }

    .contact-method {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 15px;
      background: rgba(255,255,255,0.05);
      padding: 15px 25px;
      border-radius: 10px;
      min-width: 280px;
      transition: transform 0.3s;
    }

    .contact-method:hover {
      transform: translateY(-5px);
      background: rgba(255,255,255,0.1);
    }

    .contact-icon {
      width: 40px;
      height: 40px;
      border-radius: 50%;
      background: rgba(0, 230, 118, 0.1);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 18px;
      color: #00e676;
    }

    .contact-details h3 {
      color: #fff;
      margin-bottom: 2px;
      font-size: 16px;
      text-align: left;
    }

    .contact-details a {
      color: #c9d1d9;
      text-decoration: none;
      transition: color 0.3s;
      font-size: 14px;
      text-align: left;
      display: block;
    }

    .contact-details a:hover {
      color: #00e676;
    }

    /* Footer */
    footer {
      background: #000;
      padding: 30px 0 15px;
      text-align: center;
    }

    .footer-content {
      display: flex;
      flex-direction: column;
      gap: 20px;
      margin-bottom: 20px;
    }

    .social-links {
      display: flex;
      justify-content: center;
      gap: 15px;
    }

    .social-links a {
      width: 40px;
      height: 40px;
      border-radius: 50%;
      background: #161b22;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      text-decoration: none;
      transition: all 0.3s;
    }

    .social-links a:hover {
      background: #00e676;
      transform: translateY(-3px);
      color: #000;
    }

    .copyright {
      border-top: 1px solid rgba(255, 255, 255, 0.1);
      padding-top: 15px;
      font-size: 14px;
      color: #c9d1d9;
    }

    /* WhatsApp Float */
    .whatsapp-float {
      position: fixed;
      width: 60px;
      height: 60px;
      bottom: 20px;
      right: 20px;
      background: #25D366;
      color: white;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 24px;
      box-shadow: 0 4px 15px rgba(37, 211, 102, 0.4);
      text-decoration: none;
      z-index: 1000;
      transition: all 0.3s;
    }

    .whatsapp-float:hover {
      transform: scale(1.1);
      box-shadow: 0 6px 20px rgba(37, 211, 102, 0.6);
    }

    /* Responsive Design */
    @media (max-width: 768px) {
      .hamburger {
        display: block;
      }

      .nav-menu {
        position: fixed;
        top: 70px;
        right: -100%;
        background: #0d1117;
        flex-direction: column;
        width: 250px;
        height: 100vh;
        padding: 40px 20px;
        transition: right 0.3s;
        box-shadow: -5px 0 15px rgba(0, 0, 0, 0.3);
      }

      .nav-menu.active {
        right: 0;
      }

      .hero h1 {
        font-size: 2rem;
      }
      
      .card {
        width: 100%;
        max-width: 300px;
      }
    }
  </style>
</head>
<body>
  <div class="animated-bg" id="animatedBg"></div>

  <header>
    <div class="nav-container">
      <a href="#" class="logo">Mohit<span>Prasad</span></a>
      
      <div class="hamburger" id="hamburger">
        <i class="fas fa-bars"></i>
      </div>
      
      <ul class="nav-menu" id="navMenu">
        <li><a href="#home">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </div>
  </header>

  <section class="hero" id="home">
    <div class="hero-content">
      <h1>Master Practical Skills for Career Growth</h1>
      <p>Affordable & Practical Training in MS Excel, Stock Market, Crypto Trading, Freelancing & Basic Computer in Delhi.</p>
      <div class="hero-buttons">
        <a href="#services" class="btn">Explore Courses</a>
        <a href="#contact" class="btn btn-secondary">Contact Now</a>
      </div>
    </div>
  </section>

  <section id="services">
    <div class="section-title">
      <h2>Our Services</h2>
      <p>10+ Comprehensive training programs to boost your career</p>
    </div>
    
    <div class="card-container">
      <div class="card">
        <div class="card-front">
          <div class="card-image">
            <img src="https://images.unsplash.com/photo-1611224923853-80b023f02d71?auto=format&fit=crop&w=600&q=80" alt="MS Excel">
          </div>
          <h3>MS Excel Mastery</h3>
          <p>From basic functions to advanced data analysis</p>
          <p style="color: #00e676; font-size: 12px;">Tap for details</p>
        </div>
        <div class="card-back">
          <h3>MS Excel Mastery</h3>
          <ul class="features">
            <li>Formulas and Functions</li>
            <li>Data Visualization</li>
            <li>Pivot Tables & Analysis</li>
            <li>Real-world Projects</li>
            <li>Certification</li>
          </ul>
        </div>
      </div>

      <div class="card">
        <div class="card-front">
          <div class="card-image">
            <img src="https://images.unsplash.com/photo-1611974789855-9c2a0a7236a3?auto=format&fit=crop&w=600&q=80" alt="Stock Market">
          </div>
          <h3>Stock Market Trading</h3>
          <p>Learn proven strategies for stock trading</p>
          <p style="color: #00e676; font-size: 12px;">Tap for details</p>
        </div>
        <div class="card-back">
          <h3>Stock Market Trading</h3>
          <ul class="features">
            <li>Market Fundamentals</li>
            <li>Technical Analysis</li>
            <li>Risk Management</li>
            <li>Portfolio Building</li>
            <li>Live Trading Sessions</li>
          </ul>
        </div>
      </div>

      <div class="card">
        <div class="card-front">
          <div class="card-image">
            <img src="https://images.unsplash.com/photo-1620336655055-bd87ca8f1370?auto=format&fit=crop&w=600&q=80" alt="Crypto Trading">
          </div>
          <h3>Crypto Trading</h3>
          <p>Navigate the world of cryptocurrency</p>
          <p style="color: #00e676; font-size: 12px;">Tap for details</p>
        </div>
        <div class="card-back">
          <h3>Crypto Trading</h3>
          <ul class="features">
            <li>Crypto Fundamentals</li>
            <li>Exchange Platforms</li>
            <li>Wallet Management</li>
            <li>Trading Strategies</li>
            <li>Risk Assessment</li>
          </ul>
        </div>
      </div>

      <div class="card">
        <div class="card-front">
          <div class="card-image">
            <img src="https://images.unsplash.com/photo-1573164713714-d95e436ab8d6?auto=format&fit=crop&w=600&q=80" alt="Freelancing">
          </div>
          <h3>Freelancing</h3>
          <p>Build a successful freelancing career</p>
          <p style="color: #00e676; font-size: 12px;">Tap for details</p>
        </div>
        <div class="card-back">
          <h3>Freelancing</h3>
          <ul class="features">
            <li>Platform Setup</li>
            <li>Profile Optimization</li>
            <li>Client Acquisition</li>
            <li>Project Pricing</li>
            <li>Portfolio Development</li>
          </ul>
        </div>
      </div>

      <div class="card">
        <div class="card-front">
          <div class="card-image">
            <img src="https://images.unsplash.com/photo-1542831371-29b0f74f9713?auto=format&fit=crop&w=600&q=80" alt="Basic Computer">
          </div>
          <h3>Basic Computer Skills</h3>
          <p>Essential computer literacy</p>
          <p style="color: #00e676; font-size: 12px;">Tap for details</p>
        </div>
        <div class="card-back">
          <h3>Basic Computer Skills</h3>
          <ul class="features">
            <li>OS Navigation</li>
            <li>MS Office Suite</li>
            <li>Internet & Email</li>
            <li>File Management</li>
            <li>Basic Troubleshooting</li>
          </ul>
        </div>
      </div>

      <div class="card">
        <div class="card-front">
          <div class="card-image">
            <img src="https://images.unsplash.com/photo-1533750516457-a7f992034fec?auto=format&fit=crop&w=600&q=80" alt="Digital Marketing">
          </div>
          <h3>Digital Marketing</h3>
          <p>Master SEO, Social Media & Ads</p>
          <p style="color: #00e676; font-size: 12px;">Tap for details</p>
        </div>
        <div class="card-back">
          <h3>Digital Marketing</h3>
          <ul class="features">
            <li>SEO Optimization</li>
            <li>Social Media Marketing</li>
            <li>Google Ads</li>
            <li>Content Strategy</li>
            <li>Analytics & Growth</li>
          </ul>
        </div>
      </div>

      <div class="card">
        <div class="card-front">
          <div class="card-image">
            <img src="https://images.unsplash.com/photo-1626785774573-4b79931256ce?auto=format&fit=crop&w=600&q=80" alt="Graphic Design">
          </div>
          <h3>Graphic Design</h3>
          <p>Create stunning visuals with Canva & PS</p>
          <p style="color: #00e676; font-size: 12px;">Tap for details</p>
        </div>
        <div class="card-back">
          <h3>Graphic Design</h3>
          <ul class="features">
            <li>Color Theory</li>
            <li>Logo Design</li>
            <li>Social Media Posts</li>
            <li>Canva & Photoshop</li>
            <li>Portfolio Building</li>
          </ul>
        </div>
      </div>

      <div class="card">
        <div class="card-front">
          <div class="card-image">
            <img src="https://images.unsplash.com/photo-1536240478700-b869070f9279?auto=format&fit=crop&w=600&q=80" alt="Video Editing">
          </div>
          <h3>Video Editing</h3>
          <p>Edit videos for YouTube & Reels</p>
          <p style="color: #00e676; font-size: 12px;">Tap for details</p>
        </div>
        <div class="card-back">
          <h3>Video Editing</h3>
          <ul class="features">
            <li>Timeline Management</li>
            <li>Transitions & Effects</li>
            <li>Color Grading</li>
            <li>Audio Mixing</li>
            <li>Exporting Formats</li>
          </ul>
        </div>
      </div>

      <div class="card">
        <div class="card-front">
          <div class="card-image">
            <img src="https://images.unsplash.com/photo-1587620962725-abab7fe55159?auto=format&fit=crop&w=600&q=80" alt="Web Development">
          </div>
          <h3>Web Development</h3>
          <p>Build your own websites from scratch</p>
          <p style="color: #00e676; font-size: 12px;">Tap for details</p>
        </div>
        <div class="card-back">
          <h3>Web Development</h3>
          <ul class="features">
            <li>HTML5 Structure</li>
            <li>CSS3 Styling</li>
            <li>Responsive Design</li>
            <li>Basic JavaScript</li>
            <li>Hosting & Domains</li>
          </ul>
        </div>
      </div>

      <div class="card">
        <div class="card-front">
          <div class="card-image">
            <img src="https://images.unsplash.com/photo-1526374965328-7f61d4dc18c5?auto=format&fit=crop&w=600&q=80" alt="Python Programming">
          </div>
          <h3>Python Programming</h3>
          <p>Learn coding and automation</p>
          <p style="color: #00e676; font-size: 12px;">Tap for details</p>
        </div>
        <div class="card-back">
          <h3>Python Programming</h3>
          <ul class="features">
            <li>Python Basics</li>
            <li>Data Structures</li>
            <li>Loops & Functions</li>
            <li>Web Scraping</li>
            <li>Automating Tasks</li>
          </ul>
        </div>
      </div>

    </div>
  </section>

  <section class="contact" id="contact">
    <div class="section-title">
      <h2>Contact Me</h2>
      <p>Reach out to discuss which course is right for you</p>
    </div>
    
    <div class="contact-container">
      <div class="contact-method">
        <div class="contact-icon">
          <i class="fas fa-envelope"></i>
        </div>
        <div class="contact-details">
          <h3>Email</h3>
          <a href="mailto:mohitparsad371@gmail.com">mohitparsad371@gmail.com</a>
        </div>
      </div>
      
      <div class="contact-method">
        <div class="contact-icon">
          <i class="fas fa-phone"></i>
        </div>
        <div class="contact-details">
          <h3>Phone</h3>
          <a href="tel:+918595366682">+91 8595366682</a>
        </div>
      </div>
      
      <div class="contact-method">
        <div class="contact-icon">
          <i class="fab fa-whatsapp"></i>
        </div>
        <div class="contact-details">
          <h3>WhatsApp</h3>
          <a href="https://wa.me/918595366682" target="_blank">Message directly</a>
        </div>
      </div>

      <div class="contact-method">
        <div class="contact-icon">
          <i class="fab fa-instagram"></i>
        </div>
        <div class="contact-details">
          <h3>Instagram</h3>
          <a href="https://www.instagram.com/mohit_shah0002?igsh=bDU5NHM3ZTF2cTVj" target="_blank">Follow on Insta</a>
        </div>
      </div>

      <div class="contact-method">
        <div class="contact-icon">
          <i class="fab fa-twitter"></i>
        </div>
        <div class="contact-details">
          <h3>Twitter (X)</h3>
          <a href="https://x.com/element_syco?t=dmRw9UEZRQXuEy_S4iBe_g&s=09" target="_blank">F