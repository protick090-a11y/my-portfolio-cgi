<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CGI Artist Portfolio</title>

<style>
/* =====================
   GLOBAL STYLES
===================== */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background-color: #0b0b0b;
    color: #e5e5e5;
    line-height: 1.6;
}

/* =====================
   NAVBAR
===================== */
header {
    background: #000;
    padding: 20px 50px;
    position: sticky;
    top: 0;
    z-index: 100;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

nav h1 {
    color: #d4af37;
    font-size: 24px;
    letter-spacing: 2px;
}

nav ul {
    list-style: none;
    display: flex;
    gap: 30px;
}

nav ul li a {
    text-decoration: none;
    color: #e5e5e5;
    font-weight: 500;
    transition: 0.3s;
}

nav ul li a:hover {
    color: #d4af37;
}

/* =====================
   HERO SECTION
===================== */
.hero {
    height: 90vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 20px;
}

.hero h2 {
    font-size: 50px;
    color: #d4af37;
}

.hero p {
    max-width: 700px;
    margin: 20px auto;
    font-size: 18px;
}

.hero a {
    display: inline-block;
    margin-top: 25px;
    padding: 12px 35px;
    background: #d4af37;
    color: #000;
    text-decoration: none;
    font-weight: 600;
    border-radius: 30px;
    transition: 0.3s;
}

.hero a:hover {
    background: #b8962e;
}

/* =====================
   SECTION STYLES
===================== */
section {
    padding: 80px 50px;
}

.section-title {
    text-align: center;
    margin-bottom: 50px;
}

.section-title h2 {
    font-size: 36px;
    color: #d4af37;
}

/* =====================
   GALLERY
===================== */
.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 25px;
}

.gallery div {
    background: #111;
    height: 220px;
    border-radius: 10px;
    overflow: hidden;
    position: relative;
    cursor: pointer;
    transition: 0.4s;
}

.gallery div:hover {
    transform: scale(1.05);
}

.gallery div::after {
    content: "View Project";
    position: absolute;
    inset: 0;
    background: rgba(0,0,0,0.7);
    color: #d4af37;
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: 0.4s;
    font-weight: 600;
}

.gallery div:hover::after {
    opacity: 1;
}

/* =====================
   ABOUT
===================== */
.about {
    max-width: 900px;
    margin: auto;
    text-align: center;
}

.about p {
    font-size: 18px;
}

/* =====================
   CONTACT
===================== */
.contact {
    max-width: 700px;
    margin: auto;
    text-align: center;
}

.contact p {
    margin-bottom: 10px;
}

.contact a {
    color: #d4af37;
    text-decoration: none;
    font-weight: 600;
}

/* =====================
   FOOTER
===================== */
footer {
    background: #000;
    text-align: center;
    padding: 20px;
    color: #777;
    font-size: 14px;
}

/* =====================
   RESPONSIVE
===================== */
@media (max-width: 768px) {
    nav ul {
        display: none;
    }

    .hero h2 {
        font-size: 36px;
    }

    section {
        padding: 60px 20px;
    }
}
</style>
</head>

<body>

<!-- NAVBAR -->
<header>
    <nav>
        <h1>CGI ARTIST</h1>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#work">My Work</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

<!-- HERO -->
<section class="hero" id="home">
    <div>
        <h2>High-End CGI & AI Visuals</h2>
        <p>
            I create cinematic CGI visuals, product animations, and AI-powered designs
            that elevate brands and capture attention.
        </p>
        <a href="#work">View My Work</a>
    </div>
</section>

<!-- WORK -->
<section id="work">
    <div class="section-title">
        <h2>My Work</h2>
    </div>
    <div class="gallery">
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
    </div>
</section>

<!-- ABOUT -->
<section id="about">
    <div class="section-title">
        <h2>About Me</h2>
    </div>
    <div class="about">
        <p>
            I am a professional CGI Artist specializing in hyper-realistic product visuals,
            cinematic animations, and AI-generated creative content. My goal is to help
            brands stand out with visually stunning and high-conversion visuals.
        </p>
    </div>
</section>

<!-- CONTACT -->
<section id="contact">
    <div class="section-title">
        <h2>Contact</h2>
    </div>
    <div class="contact">
        <p>Email: <a href="mailto:yourname@email.com">yourname@email.com</a></p>
        <p>Instagram: <a href="#">@yourhandle</a></p>
        <p>Behance / Portfolio Link</p>
    </div>
</section>

<!-- FOOTER -->
<footer>
    © 2026 CGI Artist Portfolio. All Rights Reserved.
</footer>

</body>
</html>
