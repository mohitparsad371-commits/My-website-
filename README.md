<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Mohit Prasad Services | Learn Skills. Build. Grow.</title>

<meta name="description" content="Mohit Prasad Services offers practical training in Excel, digital skills, freelancing, web development, design, trading education and more.">
<meta name="keywords" content="MS Excel training, freelancing course, digital marketing, web development, computer course, trading education, Delhi">
<meta name="author" content="Mohit Prasad">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Space+Grotesk:wght@500;600;700&display=swap" rel="stylesheet">

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

<style>
:root{
  --bg:#05070b;
  --bg2:#0a0f17;
  --card:rgba(255,255,255,.055);
  --border:rgba(255,255,255,.10);
  --text:#f5f7fa;
  --muted:#9ba6b5;
  --green:#00e676;
  --green2:#00b85c;
  --cyan:#00d9ff;
  --purple:#8b5cf6;
  --shadow:0 25px 80px rgba(0,0,0,.45);
}

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

html{
  scroll-behavior:smooth;
}

body{
  font-family:Inter,sans-serif;
  background:
    radial-gradient(circle at 10% 10%,rgba(0,230,118,.09),transparent 30%),
    radial-gradient(circle at 90% 20%,rgba(139,92,246,.08),transparent 28%),
    var(--bg);
  color:var(--text);
  overflow-x:hidden;
}

a{
  color:inherit;
  text-decoration:none;
}

.container{
  width:min(1180px,92%);
  margin:auto;
}

/* ================= HEADER ================= */

header{
  position:fixed;
  top:0;
  left:0;
  width:100%;
  z-index:999;
  background:rgba(5,7,11,.72);
  backdrop-filter:blur(18px);
  border-bottom:1px solid rgba(255,255,255,.07);
}

.nav{
  height:76px;
  display:flex;
  align-items:center;
  justify-content:space-between;
}

.logo{
  font-family:"Space Grotesk",sans-serif;
  font-size:23px;
  font-weight:700;
  letter-spacing:-1px;
}

.logo span{
  color:var(--green);
}

.nav-links{
  display:flex;
  align-items:center;
  gap:32px;
  list-style:none;
}

.nav-links a{
  color:#b9c1cd;
  font-size:14px;
  font-weight:600;
  transition:.3s;
}

.nav-links a:hover{
  color:var(--green);
}

.nav-cta{
  padding:11px 19px;
  border:1px solid rgba(0,230,118,.4);
  border-radius:100px;
  color:var(--green)!important;
}

.menu{
  display:none;
  font-size:24px;
  cursor:pointer;
}

/* ================= HERO ================= */

.hero{
  min-height:100vh;
  display:flex;
  align-items:center;
  padding:140px 0 90px;
  position:relative;
}

.grid-bg{
  position:absolute;
  inset:0;
  pointer-events:none;
  opacity:.35;
  background-image:
    linear-gradient(rgba(255,255,255,.035) 1px,transparent 1px),
    linear-gradient(90deg,rgba(255,255,255,.035) 1px,transparent 1px);
  background-size:55px 55px;
  mask-image:linear-gradient(to bottom,#000,transparent 85%);
}

.glow{
  position:absolute;
  width:500px;
  height:500px;
  border-radius:50%;
  background:rgba(0,230,118,.08);
  filter:blur(100px);
  right:-150px;
  top:100px;
}

.hero-content{
  position:relative;
  z-index:2;
  max-width:850px;
}

.badge{
  display:inline-flex;
  align-items:center;
  gap:9px;
  padding:8px 14px;
  border:1px solid rgba(0,230,118,.22);
  background:rgba(0,230,118,.06);
  color:#8fffc0;
  border-radius:100px;
  font-size:12px;
  font-weight:700;
  margin-bottom:25px;
}

.badge i{
  font-size:8px;
}

.hero h1{
  font-family:"Space Grotesk",sans-serif;
  font-size:clamp(48px,7vw,86px);
  line-height:.98;
  letter-spacing:-4px;
  margin-bottom:27px;
}

.hero h1 span{
  background:linear-gradient(90deg,var(--green),#6dffad,var(--cyan));
  -webkit-background-clip:text;
  color:transparent;
}

.hero-text{
  color:var(--muted);
  max-width:680px;
  font-size:18px;
  line-height:1.8;
  margin-bottom:34px;
}

.hero-buttons{
  display:flex;
  gap:14px;
  flex-wrap:wrap;
}

.btn{
  display:inline-flex;
  align-items:center;
  justify-content:center;
  gap:10px;
  padding:15px 23px;
  border-radius:12px;
  font-weight:700;
  font-size:14px;
  transition:.3s;
}

.btn-primary{
  color:#001108;
  background:var(--green);
  box-shadow:0 10px 35px rgba(0,230,118,.18);
}

.btn-primary:hover{
  transform:translateY(-3px);
  box-shadow:0 15px 45px rgba(0,230,118,.3);
}

.btn-outline{
  border:1px solid var(--border);
  background:rgba(255,255,255,.035);
}

.btn-outline:hover{
  border-color:rgba(0,230,118,.4);
  color:var(--green);
  transform:translateY(-3px);
}

/* ================= STATS ================= */

.stats{
  margin-top:70px;
  display:flex;
  gap:45px;
  flex-wrap:wrap;
}

.stat h3{
  font-family:"Space Grotesk";
  font-size:28px;
}

.stat p{
  color:var(--muted);
  font-size:12px;
  margin-top:4px;
}

/* ================= SECTION ================= */

section{
  padding:105px 0;
}

.section-head{
  text-align:center;
  max-width:700px;
  margin:0 auto 55px;
}

.eyebrow{
  color:var(--green);
  font-size:12px;
  font-weight:800;
  letter-spacing:2px;
  text-transform:uppercase;
  margin-bottom:13px;
}

.section-head h2{
  font-family:"Space Grotesk";
  font-size:clamp(34px,5vw,55px);
  letter-spacing:-2px;
  margin-bottom:15px;
}

.section-head p{
  color:var(--muted);
  line-height:1.7;
}

/* ================= SERVICES ================= */

.services-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:18px;
}

.service-card{
  position:relative;
  min-height:310px;
  padding:27px;
  border:1px solid var(--border);
  border-radius:22px;
  background:linear-gradient(145deg,rgba(255,255,255,.065),rgba(255,255,255,.025));
  overflow:hidden;
  transition:.4s;
}

.service-card:before{
  content:"";
  position:absolute;
  width:170px;
  height:170px;
  background:rgba(0,230,118,.08);
  filter:blur(60px);
  right:-80px;
  top:-80px;
}

.service-card:hover{
  transform:translateY(-8px);
  border-color:rgba(0,230,118,.3);
  box-shadow:var(--shadow);
}

.icon{
  width:52px;
  height:52px;
  border-radius:15px;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:21px;
  color:var(--green);
  background:rgba(0,230,118,.08);
  border:1px solid rgba(0,230,118,.14);
  margin-bottom:25px;
}

.service-card h3{
  font-family:"Space Grotesk";
  font-size:21px;
  margin-bottom:11px;
}

.service-card p{
  color:var(--muted);
  font-size:14px;
  line-height:1.7;
  margin-bottom:22px;
}

.learn{
  color:var(--green);
  font-size:13px;
  font-weight:700;
}

/* ================= FEATURE ================= */

.feature{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:70px;
  align-items:center;
}

.feature-box{
  position:relative;
  min-height:450px;
  border-radius:28px;
  border:1px solid var(--border);
  background:
    radial-gradient(circle at 30% 20%,rgba(0,230,118,.12),transparent 35%),
    linear-gradient(145deg,#101720,#070a0f);
  overflow:hidden;
  box-shadow:var(--shadow);
}

.feature-box:after{
  content:"";
  position:absolute;
  width:250px;
  height:250px;
  border:1px solid rgba(0,230,118,.2);
  border-radius:50%;
  left:50%;
  top:50%;
  transform:translate(-50%,-50%);
  box-shadow:
    0 0 0 50px rgba(0,230,118,.025),
    0 0 0 100px rgba(0,230,118,.018);
}

.dashboard{
  position:absolute;
  z-index:2;
  width:75%;
  padding:22px;
  border:1px solid rgba(255,255,255,.1);
  background:rgba(255,255,255,.06);
  backdrop-filter:blur(15px);
  border-radius:18px;
  left:12.5%;
  top:23%;
}

.dash-top{
  display:flex;
  justify-content:space-between;
  margin-bottom:25px;
}

.dots{
  display:flex;
  gap:5px;
}

.dots span{
  width:6px;
  height:6px;
  background:#657080;
  border-radius:50%;
}

.chart{
  height:110px;
  display:flex;
  align-items:flex-end;
  gap:8px;
}

.bar{
  flex:1;
  background:linear-gradient(to top,var(--green),rgba(0,230,118,.15));
  border-radius:5px 5px 0 0;
}

.feature-content h2{
  font-family:"Space Grotesk";
  font-size:48px;
  letter-spacing:-2px;
  margin-bottom:20px;
}

.feature-content p{
  color:var(--muted);
  line-height:1.8;
  margin-bottom:25px;
}

.checks{
  list-style:none;
  display:grid;
  gap:13px;
  margin-bottom:30px;
}

.checks li{
  color:#cbd2db;
  font-size:14px;
}

.checks i{
  color:var(--green);
  margin-right:9px;
}

/* ================= PROCESS ================= */

.process{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:15px;
}

.process-card{
  padding:25px;
  border:1px solid var(--border);
  border-radius:18px;
  background:rgba(255,255,255,.03);
}

.number{
  color:var(--green);
  font-family:"Space Grotesk";
  font-size:13px;
  margin-bottom:28px;
}

.process-card h3{
  font-size:17px;
  margin-bottom:10px;
}

.process-card p{
  color:var(--muted);
  font-size:13px;
  line-height:1.7;
}

/* ================= TESTIMONIAL ================= */

.testimonials{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:18px;
}

.testimonial{
  padding:27px;
  border:1px solid var(--border);
  background:rgba(255,255,255,.035);
  border-radius:20px;
}

.stars{
  color:#ffd166;
  font-size:12px;
  margin-bottom:18px;
}

.testimonial p{
  color:#c4ccd6;
  line-height:1.8;
  font-size:14px;
  margin-bottom:25px;
}

.user{
  display:flex;
  align-items:center;
  gap:12px;
}

.avatar{
  width:40px;
  height:40px;
  border-radius:50%;
  display:flex;
  align-items:center;
  justify-content:center;
  background:rgba(0,230,118,.1);
  color:var(--green);
  font-weight:800;
}

.user small{
  color:var(--muted);
}

/* ================= CTA ================= */

.cta{
  position:relative;
  text-align:center;
  padding:75px 30px;
  border:1px solid rgba(0,230,118,.18);
  border-radius:30px;
  overflow:hidden;
  background:
    radial-gradient(circle at 50% 0%,rgba(0,230,118,.13),transparent 45%),
    rgba(255,255,255,.025);
}

.cta h2{
  font-family:"Space Grotesk";
  font-size:clamp(35px,5vw,58px);
  letter-spacing:-2px;
  margin-bottom:15px;
}

.cta p{
  color:var(--muted);
  max-width:600px;
  margin:0 auto 28px;
}

/* ================= FAQ ================= */

.faq{
  max-width:800px;
  margin:auto;
}

details{
  border-bottom:1px solid var(--border);
  padding:20px 0;
}

summary{
  cursor:pointer;
  font-weight:700;
  list-style:none;
  display:flex;
  justify-content:space-between;
}

summary:after{
  content:"+";
  color:var(--green);
}

details[open] summary:after{
  content:"−";
}

details p{
  color:var(--muted);
  font-size:14px;
  line-height:1.8;
  padding-top:15px;
}

/* ================= CONTACT ================= */

.contact-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:20px;
}

.contact-card{
  display:flex;
  align-items:center;
  gap:17px;
  padding:22px;
  border:1px solid var(--border);
  border-radius:17px;
  background:rgba(255,255,255,.035);
  transition:.3s;
}

.contact-card:hover{
  border-color:rgba(0,230,118,.3);
  transform:translateY(-4px);
}

.contact-card .icon{
  margin:0;
  flex-shrink:0;
}

.contact-card h3{
  font-size:14px;
  margin-bottom:4px;
}

.contact-card p{
  color:var(--muted);
  font-size:13px;
}

/* ================= FOOTER ================= */

footer{
  border-top:1px solid var(--border);
  padding:50px 0 25px;
}

.footer-top{
  display:flex;
  justify-content:space-between;
  align-items:center;
  gap:30px;
  margin-bottom:40px;
}

.footer-top p{
  color:var(--muted);
  font-size:13px;
  margin-top:7px;
}

.socials{
  display:flex;
  gap:9px;
}

.socials a{
  width:40px;
  height:40px;
  border:1px solid var(--border);
  border-radius:50%;
  display:flex;
  align-items:center;
  justify-content:center;
  color:#b8c0ca;
  transition:.3s;
}

.socials a:hover{
  color:#001108;
  background:var(--green);
  border-color:var(--green);
  transform:translateY(-3px);
}

.copyright{
  padding-top:20px;
  border-top:1px solid var(--border);
  color:#687382;
  font-size:12px;
  text-align:center;
}

/* ================= WHATSAPP ================= */

.whatsapp{
  position:fixed;
  right:22px;
  bottom:22px;
  width:58px;
  height:58px;
  border-radius:50%;
  background:#25d366;
  color:white;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:25px;
  z-index:1000;
  box-shadow:0 10px 35px rgba(37,211,102,.35);
  animation:pulse 2s infinite;
}

@keyframes pulse{
  0%,100%{box-shadow:0 10px 35px rgba(37,211,102,.3)}
  50%{box-shadow:0 10px 50px rgba(37,211,102,.6)}
}

/* ================= RESPONSIVE ================= */

@media(max-width:900px){

  .services-grid{
    grid-template-columns:repeat(2,1fr);
  }

  .feature{
    grid-template-columns:1fr;
  }

  .process{
    grid-template-columns:repeat(2,1fr);
  }

  .testimonials{
    grid-template-columns:1fr;
  }
}

@media(max-width:700px){

  .nav{
    height:68px;
  }

  .menu{
    display:block;
  }

  .nav-links{
    position:absolute;
    top:68px;
    right:-100%;
    width:270px;
    height:calc(100vh - 68px);
    background:#070a0f;
    padding:35px 25px;
    flex-direction:column;
    align-items:flex-start;
    gap:25px;
    transition:.35s;
    border-left:1px solid var(--border);
  }

  .nav-links.active{
    right:0;
  }

  .hero{
    padding-top:125px;
  }

  .hero h1{
    font-size:48px;
    letter-spacing:-2.5px;
  }

  .hero-text{
    font-size:15px;
  }

  .stats{
    gap:25px;
  }

  section{
    padding:75px 0;
  }

  .services-grid,
  .contact-grid,
  .process{
    grid-template-columns:1fr;
  }

  .feature-content h2{
    font-size:38px;
  }

  .feature-box{
    min-height:350px;
  }

  .footer-top{
    flex-direction:column;
    align-items:flex-start;
  }
}

@media(max-width:430px){

  .hero h1{
    font-size:41px;
  }

  .hero-buttons .btn{
    width:100%;
  }

  .stats{
    display:grid;
    grid-template-columns:1fr 1fr;
  }

  .service-card{
    min-height:280px;
  }
}
</style>
</head>

<body>

<header>
  <div class="container nav">

    <a href="#home" class="logo">
      Mohit<span>Prasad</span>
    </a>

    <div class="menu" id="menu">
      <i class="fa-solid fa-bars"></i>
    </div>

    <ul class="nav-links" id="navLinks">
      <li><a href="#home">Home</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#process">How It Works</a></li>
      <li><a href="#faq">FAQ</a></li>
      <li><a href="#contact">Contact</a></li>
      <li>
        <a class="nav-cta"
           href="https://wa.me/918595366682"
           target="_blank">
          Let's Talk
        </a>
      </li>
    </ul>

  </div>
</header>


<!-- HERO -->

<section class="hero" id="home">

  <div class="grid-bg"></div>
  <div class="glow"></div>

  <div class="container">
    <div class="hero-content">

      <div class="badge">
        <i class="fa-solid fa-circle"></i>
        PRACTICAL SKILLS. REAL-WORLD RESULTS.
      </div>

      <h1>
        Learn Skills That
        <span>Actually Move</span>
        Your Career Forward.
      </h1>

      <p class="hero-text">
        Practical, beginner-friendly training designed to help you
        learn useful digital skills, build confidence and create
        real-world opportunities.
      </p>

      <div class="hero-buttons">

        <a href="#services" class="btn btn-primary">
          Explore Programs
          <i class="fa-solid fa-arrow-right"></i>
        </a>

        <a href="https://wa.me/918595366682?text=Hi%20Mohit%2C%20I%20want%20to%20know%20about%20your%20courses."
           target="_blank"
           class="btn btn-outline">
          <i class="fa-brands fa-whatsapp"></i>
          Talk on WhatsApp
        </a>

      </div>

      <div class="stats">

        <div class="stat">
          <h3>10+</h3>
          <p>Skill Programs</p>
        </div>

        <div class="stat">
          <h3>100%</h3>
          <p>Practical Focus</p>
        </div>

        <div class="stat">
          <h3>1:1</h3>
          <p>Personal Guidance</p>
        </div>

      </div>

    </div>
  </div>
</section>


<!-- SERVICES -->

<section id="services">

  <div class="container">

    <div class="section-head">
      <div class="eyebrow">What I Teach</div>

      <h2>Skills Built For The Real World.</h2>

      <p>
        No unnecessary theory. Learn useful skills through practical
        concepts, tools, examples and projects.
      </p>
    </div>


    <div class="services-grid">

      <div class="service-card">
        <div class="icon">
          <i class="fa-solid fa-table"></i>
        </div>

        <h3>MS Excel Mastery</h3>

        <p>
          From basic formulas to advanced functions, data cleaning,
          dashboards, Pivot Tables and practical business tasks.
        </p>

        <span class="learn">Learn Excel →</span>
      </div>


      <div class="service-card">
        <div class="icon">
          <i class="fa-solid fa-chart-line"></i>
        </div>

        <h3>Stock Market Education</h3>

        <p>
          Understand market basics, technical concepts, charts,
          risk management and disciplined decision-making.
        </p>

        <span class="learn">Explore Trading →</span>
      </div>


      <div class="service-card">
        <div class="icon">
          <i class="fa-brands fa-bitcoin"></i>
        </div>

        <h3>Crypto Education</h3>

        <p>
          Learn blockchain basics, exchanges, wallets, market concepts
          and responsible risk management.
        </p>

        <span class="learn">Explore Crypto →</span>
      </div>


      <div class="service-card">
        <div class="icon">
          <i class="fa-solid fa-laptop-code"></i>
        </div>

        <h3>Web Development</h3>

        <p>
          Learn HTML, CSS, responsive design and JavaScript fundamentals
          while building real websites.
        </p>

        <span class="learn">Start Building →</span>
      </div>


      <div class="service-card">
        <div class="icon">
          <i class="fa-solid fa-pen-nib"></i>
        </div>

        <h3>Graphic Design</h3>

        <p>
          Learn Canva, Photoshop fundamentals, layouts, branding,
          social media creatives and portfolio creation.
        </p>

        <span class="learn">Design Better →</span>
      </div>


      <div class="service-card">
        <div class="icon">
          <i class="fa-solid fa-video"></i>
        </div>

        <h3>Video Editing</h3>

        <p>
          Create engaging videos for YouTube, Instagram and short-form
          platforms with practical editing workflows.
        </p>

        <span class="learn">Start Editing →</span>
      </div>


      <div class="service-card">
        <div class="icon">
          <i class="fa-solid fa-bullhorn"></i>
        </div>

        <h3>Digital Marketing</h3>

        <p>
          Understand SEO, social media, content strategy, advertising
          fundamentals and analytics.
        </p>

        <span class="learn">Grow Online →</span>
      </div>


      <div class="service-card">
        <div class="icon">
          <i class="fa-solid fa-briefcase"></i>
        </div>

        <h3>Freelancing</h3>

        <p>
          Learn how to build a profile, create a portfolio, communicate
          with clients and structure your services.
        </p>

        <span class="learn">Go Freelance →</span>
      </div>


      <div class="service-card">
        <div class="icon">
          <i class="fa-solid fa-computer"></i>
        </div>

        <h3>Basic Computer Skills</h3>

        <p>
          Build confidence with computers, files, MS Office, internet,
          email and everyday digital tasks.
        </p>

        <span class="learn">Build Basics →</span>
      </div>


      <div class="service-card">
        <div class="icon">
          <i class="fa-brands fa-python"></i>
        </div>

        <h3>Python Programming</h3>

        <p>
          Start coding with Python fundamentals, logic, functions,
          automation concepts and practical projects.
        </p>

        <span class="learn">Learn Python →</span>
      </div>

    </div>

  </div>
</section>


<!-- FEATURE -->

<section>

  <div class="container feature">

    <div class="feature-box">

      <div class="dashboard">

        <div class="dash-top">
          <strong>Learning Progress</strong>

          <div class="dots">
            <span></span>
            <span></span>
            <span></span>
          </div>
        </div>

        <div class="chart">
          <div class="bar" style="height:35%"></div>
          <div class="bar" style="height:48%"></div>
          <div class="bar" style="height:42%"></div>
          <div class="bar" style="height:67%"></div>
          <div class="bar" style="height:60%"></div>
          <div class="bar" style="height:82%"></div>
          <div class="bar" style="height:95%"></div>
        </div>

      </div>

    </div>


    <div class="feature-content">

      <div class="eyebrow">Why Learn Here?</div>

      <h2>Don't Just Watch. Learn. Practice. Build.</h2>

      <p>
        The goal is simple: help you move from “I don't know how”
        to “I can actually do this.”
      </p>

      <ul class="checks">

        <li>
          <i class="fa-solid fa-circle-check"></i>
          Beginner-friendly explanations
        </li>

        <li>
          <i class="fa-solid fa-circle-check"></i>
          Practical examples and projects
        </li>

        <li>
          <i class="fa-solid fa-circle-check"></i>
          Step-by-step learning approach
        </li>

        <li>
          <i class="fa-solid fa-circle-check"></i>
          Career-focused digital skills
        </li>

        <li>
          <i class="fa-solid fa-circle-check"></i>
          Personal guidance and support
        </li>

      </ul>

      <a href="https://wa.me/918595366682?text=Hi%20Mohit%2C%20I%20want%20to%20start%20learning."
         target="_blank"
         class="btn btn-primary">
        Start Your Journey
        <i class="fa-solid fa-arrow-right"></i>
      </a>

    </div>

  </div>
</section>


<!-- PROCESS -->

<section id="process">

  <div class="container">

    <div class="section-head">
      <div class="eyebrow">Simple Process</div>
      <h2>From Beginner To Confident.</h2>
      <p>Four simple steps to get started.</p>
    </div>


    <div class="process">

      <div class="process-card">
        <div class="number">01 — DISCOVER</div>
        <h3>Choose Your Skill</h3>
        <p>
          Tell us what you want to learn and where you currently stand.
        </p>
      </div>

      <div class="process-card">
        <div class="number">02 — PLAN</div>
        <h3>Get A Learning Path</h3>
        <p>
          Follow a structured path designed around your learning goals.
        </p>
      </div>

      <div class="process-card">
        <div class="number">03 — PRACTICE</div>
        <h3>Work On Real Tasks</h3>
        <p>
          Turn concepts into practical skills through examples and projects.
        </p>
      </div>

      <div class="process-card">
        <div class="number">04 — BUILD</div>
        <h3>Create & Grow</h3>
        <p>
          Use your skills to build projects, improve your portfolio and grow.
        </p>
      </div>

    </div>

  </div>
</section>


<!-- TESTIMONIALS -->

<section>

  <div class="container">

    <div class="section-head">
      <div class="eyebrow">Student Experience</div>
      <h2>Learning Should Feel Practical.</h2>
      <p>
        Add genuine student feedback here as your community grows.
      </p>
    </div>


    <div class="testimonials">

      <div class="testimonial">

        <div class="stars">★★★★★</div>

        <p>
          “The explanations were simple and practical. I finally
          started understanding Excel instead of just memorising formulas.”
        </p>

        <div class="user">
          <div class="avatar">S</div>
          <div>
            <strong>Student</strong><br>
            <small>MS Excel Program</small>
          </div>
        </div>

      </div>


      <div class="testimonial">

        <div class="stars">★★★★★</div>

        <p>
          “The best part was the practical approach. Everything was
          explained step by step without making it complicated.”
        </p>

        <div class="user">
          <div class="avatar">A</div>
          <div>
            <strong>Student</strong><br>
            <small>Digital Skills</small>
          </div>
        </div>

      </div>


      <div class="testimonial">

        <div class="stars">★★★★★</div>

        <p>
          “I liked that I could ask questions and actually practice
          what I was learning.”
        </p>

        <div class="user">
          <div class="avatar">R</div>
          <div>
            <strong>Student</strong><br>
            <small>Freelancing Program</small>
          </div>
        </div>

      </div>

    </div>

  </div>
</section>


<!-- CTA -->

<section>

  <div class="container">

    <div class="cta">

      <div class="eyebrow">READY WHEN YOU ARE</div>

      <h2>Your Next Skill Starts Here.</h2>

      <p>
        Tell me what you want to learn, and let's figure out the
        right starting point for you.
      </p>

      <a href="https://wa.me/918595366682?text=Hi%20Mohit%2C%20I%20want%20to%20discuss%20a%20course."
         target="_blank"
         class="btn btn-primary">
        <i class="fa-brands fa-whatsapp"></i>
        Discuss On WhatsApp
      </a>

    </div>

  </div>
</section>


<!-- FAQ -->

<section id="faq">

  <div class="container">

    <div class="section-head">
      <div class="eyebrow">FAQ</div>
      <h2>Questions? Start Here.</h2>
    </div>


    <div class="faq">

      <details>
        <summary>Are these programs suitable for beginners?</summary>
        <p>
          Yes. Programs are structured so beginners can start from
          the fundamentals and gradually move toward practical tasks.
        </p>
      </details>

      <details>
        <summary>How do I know which program is right for me?</summary>
        <p>
          Contact us on WhatsApp with your current skill level and
          goal. We can help you identify a suitable starting point.
        </p>
      </details>

      <details>
        <summary>Do you provide practical projects?</summary>
        <p>
          Practical examples and project-based learning can be included
          depending on the selected program.
        </p>
      </details>

      <details>
        <summary>Is trading education financial advice?</summary>
        <p>
          No. Trading and crypto content is educational only and does
          not guarantee profits or replace personalised financial advice.
        </p>
      </details>

      <details>
        <summary>How can I join?</summary>
        <p>
          Simply contact us through WhatsApp and share the skill you
          want to learn.
        </p>
      </details>

    </div>

  </div>
</section>


<!-- CONTACT -->

<section id="contact">

  <div class="container">

    <div class="section-head">
      <div class="eyebrow">Let's Connect</div>
      <h2>Have A Goal? Let's Talk.</h2>
      <p>
        Reach out directly and tell us what you want to learn.
      </p>
    </div>


    <div class="contact-grid">

      <a class="contact-card"
         href="mailto:mohitparsad371@gmail.com">

        <div class="icon">
          <i class="fa-solid fa-envelope"></i>
        </div>

        <div>
          <h3>Email</h3>
          <p>mohitparsad371@gmail.com</p>
        </div>

      </a>


      <a class="contact-card"
         href="tel:+918595366682">

        <div class="icon">
          <i class="fa-solid fa-phone"></i>
        </div>

        <div>
          <h3>Phone</h3>
          <p>+91 8595366682</p>
        </div>

      </a>


      <a class="contact-card"
         href="https://wa.me/918595366682"
         target="_blank">

        <div class="icon">
          <i class="fa-brands fa-whatsapp"></i>
        </div>

        <div>
          <h3>WhatsApp</h3>
          <p>Message directly</p>
        </div>

      </a>


      <a class="contact-card"
         href="https://www.linkedin.com/in/mohit-prasad-769316336"
         target="_blank">

        <div class="icon">
          <i class="fa-brands fa-linkedin-in"></i>
        </div>

        <div>
          <h3>LinkedIn</h3>
          <p>Connect professionally</p>
        </div>

      </a>


      <a class="contact-card"
         href="https://www.instagram.com/mohit_shah0002"
         target="_blank">

        <div class="icon">
          <i class="fa-brands fa-instagram"></i>
        </div>

        <div>
          <h3>Instagram</h3>
          <p>Follow on Instagram</p>
        </div>

      </a>


      <a class="contact-card"
         href="https://x.com/element_syco"
         target="_blank">

        <div class="icon">
          <i class="fa-brands fa-x-twitter"></i>
        </div>

        <div>
          <h3>X / Twitter</h3>
          <p>Follow on X</p>
        </div>

      </a>

    </div>

  </div>
</section>


<!-- FOOTER -->

<footer>

  <div class="container">

    <div class="footer-top">

      <div>
        <div class="logo">
          Mohit<span>Prasad</span>
        </div>

        <p>
          Practical skills for real-world growth.
        </p>
      </div>


      <div class="socials">

        <a href="https://www.instagram.com/mohit_shah0002"
           target="_blank">
          <i class="fa-brands fa-instagram"></i>
        </a>

        <a href="https://www.linkedin.com/in/mohit-prasad-769316336"
           target="_blank">
          <i class="fa-brands fa-linkedin-in"></i>
        </a>

        <a href="https://x.com/element_syco"
           target="_blank">
          <i class="fa-brands fa-x-twitter"></i>
        </a>

        <a href="https://wa.me/918595366682"
           target="_blank">
          <i class="fa-brands fa-whatsapp"></i>
        </a>

      </div>

    </div>


    <div class="copyright">
      © 2026 Mohit Prasad Services. All rights reserved.
    </div>

  </div>

</footer>


<!-- WHATSAPP FLOAT -->

<a class="whatsapp"
   href="https://wa.me/918595366682?text=Hi%20Mohit%2C%20I%20visited%20your%20website%20and%20want%20to%20know%20more."
   target="_blank"
   aria-label="Chat on WhatsApp">

  <i class="fa-brands fa-whatsapp"></i>

</a>


<script>

const menu = document.getElementById("menu");
const navLinks = document.getElementById("navLinks");

menu.addEventListener("click", () => {

  navLinks.classList.toggle("active");

  const icon = menu.querySelector("i");

  if(navLinks.classList.contains("active")){
    icon.classList.replace("fa-bars","fa-xmark");
  }else{
    icon.classList.replace("fa-xmark","fa-bars");
  }

});


document.querySelectorAll(".nav-links a").forEach(link => {

  link.addEventListener("click", () => {

    navLinks.classList.remove("active");

    const icon = menu.querySelector("i");

    icon.classList.replace("fa-xmark","fa-bars");

  });

});


/* Reveal animation */

const observer = new IntersectionObserver(
(entries) => {

  entries.forEach(entry => {

    if(entry.isIntersecting){

      entry.target.style.opacity = "1";
      entry.target.style.transform = "translateY(0)";

    }

  });

},
{
  threshold:.08
});


document.querySelectorAll(
".service-card,.process-card,.testimonial,.contact-card,.feature-content"
).forEach(el => {

  el.style.opacity = "0";
  el.style.transform = "translateY(25px)";
  el.style.transition = "opacity .7s ease, transform .7s ease";

  observer.observe(el);

});

</script>

</body>
</html>
