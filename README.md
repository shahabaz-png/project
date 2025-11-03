<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Shahabas Ahammed K P | Portfolio</title>
  <style>
    /* -----------------------------
       ✨ Page Load Fade Effect
    ----------------------------- */
    html {
      scroll-behavior: smooth;
    }

    body {
      opacity: 0;
      animation: fadeInBody 1s ease forwards;
    }

    @keyframes fadeInBody {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    /* -----------------------------
       🌿 Base Styles
    ----------------------------- */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', Arial, sans-serif;
    }

    body {
      background: #f9f9f9;
      color: #333;
      line-height: 1.6;
    }

    /* -----------------------------
       🧭 Navigation Bar
    ----------------------------- */
    nav {
      background: #047857;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 50;
      backdrop-filter: blur(6px);
      transition: background 0.4s ease;
    }

    nav:hover {
      background: #065f46;
    }

    nav h1 {
      color: white;
      font-size: 1.5rem;
      letter-spacing: 1px;
    }

    nav ul {
      list-style: none;
      display: flex;
    }

    nav ul li {
      margin-left: 20px;
    }

    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: 500;
      transition: all 0.3s ease-in-out;
    }

    nav ul li a:hover {
      color: #facc15;
      transform: translateY(-2px);
    }

    /* -----------------------------
       🏠 Hero Section
    ----------------------------- */
    .hero {
      background: linear-gradient(to right, #047857, #065f46);
      color: white;
      text-align: center;
      padding: 5rem 1rem;
      animation: fadeUp 1.2s ease;
    }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .hero img {
      width: 150px;
      height: 150px;
      border-radius: 25%;
      border: 4px solid #facc15;
      margin-bottom: 1rem;
      transition: transform 0.4s ease, box-shadow 0.4s ease;
    }

    .hero img:hover {
      transform: scale(1.08) rotate(3deg);
      box-shadow: 0 8px 24px rgba(0,0,0,0.2);
    }

    .hero h2 {
      font-size: 2.2rem;
      margin-bottom: 0.6rem;
      letter-spacing: 0.5px;
    }

    .hero p {
      margin: 1rem auto;
      max-width: 600px;
      line-height: 1.5;
      opacity: 0.95;
    }

    .hero .btn {
      display: inline-block;
      background: #facc15;
      color: #065f46;
      padding: 0.8rem 1.4rem;
      margin: 0.5rem;
      border-radius: 30px;
      text-decoration: none;
      font-weight: bold;
      transition: all 0.4s ease;
    }

    .hero .btn:hover {
      background: white;
      color: #000;
      transform: translateY(-4px);
      box-shadow: 0 6px 20px rgba(0,0,0,0.2);
    }

    /* -----------------------------
       📘 Section Common Styles
    ----------------------------- */
    section {
      max-width: 1000px;
      margin: auto;
      padding: 3rem 1rem;
      animation: fadeIn 1.2s ease;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    section h2 {
      text-align: center;
      color: #06546;
      margin-bottom: 2rem;
      font-size: 1.8rem;
      position: relative;
    }

    section h2::after {
      content: '';
      width: 60px;
      height: 4px;
      background: #facc15;
      display: block;
      margin: 10px auto 0;
      border-radius: 2px;
    }

    /* -----------------------------
       👤 About Section
    ----------------------------- */
    #about p {
      text-align: center;
      max-width: 700px;
      margin: auto;
      color: #444;
      font-size: 1.05rem;
      animation: fadeIn 1.2s ease;
    }

    /* -----------------------------
       💼 Services Section
    ----------------------------- */
    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
    }

    .service-card {
      background: white;
      padding: 2rem;
      text-align: center;
      border-radius: 15px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      transition: all 0.4s ease;
    }

    .service-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
    }

    /* -----------------------------
       🏆 Projects Section
    ----------------------------- */
    .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.5rem;
    }

    .project-card {
      background: white;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      transition: all 0.4s ease;
    }

    .project-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.15);
    }

    .project-card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      transition: transform 0.5s ease;
    }

    .project-card:hover img {
      transform: scale(1.05);
    }

    .project-card p {
      padding: 1rem;
      text-align: center;
      transition: color 0.3s;
    }

    .project-card a {
      text-decoration: none;
      color: #065f46;
      font-weight: 600;
      transition: color 0.3s;
    }

    .project-card a:hover {
      color: #facc15;
    }

    /* -----------------------------
       📞 Contact Section
    ----------------------------- */
    #contact {
      text-align: center;
      animation: fadeIn 1.2s ease;
    }

    #contact a {
      color: #047857;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }

    #contact a:hover {
      color: #facc15;
    }

    /* -----------------------------
       🦶 Footer
    ----------------------------- */
    footer {
      text-align: center;
      padding: 1rem;
      background: #065f46;
      color: white;
      margin-top: 2rem;
      font-size: 0.9rem;
      letter-spacing: 0.5px;
    }
header{
  position:sticky;top:12px;z-index:40;padding:12px 0;backdrop-filter: blur(6px);
}
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav>
<header>
    <h1>Portfolio</h1>
    <ul>
      <li><a href="port2.0.html">Home</a></li>
      <li><a href="about.html">About</a></li>
      <li><a href="service.html">Services</a></li>
      <li><a href="projects.html">Projects</a></li>
      <li><a href="contact.html">Contact</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <section class="hero" id="hero">
    <img src="0.jpeg" alt="Profile Photo">
    <h2>Hi, I'm Shahabas Ahammed K P</h2>
    <p>2nd Year BCA Student | AWS Cloud & AI Data Analytics<br>Srinivas University</p>
    <a href="#contact" class="btn">Hire Me</a>
    <a href="cv.jpeg" class="btn">Download CV</a>
  </section>

  <!-- About -->
  <section id="about">
    <h2>About Me</h2>
    <p>
      I am a passionate student specializing in <b>AWS Cloud and AI Data Analytics</b> at Srinivas University.
      My interests include technology, cloud solutions, and data-driven applications.
      I love solving problems and creating impactful solutions.
    </p>
  </section>

  <!-- Services -->
  <section id="services">
    <h2>Services</h2>
    <div class="services">
      <div class="service-card">
        <h3>Web Development</h3>
        <p>Building responsive and modern websites using HTML, CSS, and JavaScript.</p>
      </div>
      <div class="service-card">
        <h3>Cloud Solutions</h3>
        <p>Basic setup and management of AWS Cloud resources for academic and small-scale projects.</p>
      </div>
      <div class="service-card">
        <h3>Data Analytics</h3>
        <p>Data analysis and visualization using Python and AI fundamentals.</p>
      </div>
    </div>
  </section>

  <!-- Projects -->
  <section id="projects">
    <h2>Achievements</h2>
    <div class="projects">
      <div class="project-card">
        <img src="6.PNG" alt="Project 1">
        <p><a href="6.PNG">Participated in national-level IT fest at Agnes College</a></p>
      </div>
      <div class="project-card">
        <img src="heloo.jpeg" alt="Project 2">
        <p><a href="heloo.jpeg">Online Course: Introduction To Artificial Intelligence</a></p>
      </div>
      <div class="project-card">
        <img src="hii.jpeg" alt="Project 3">
        <p><a href="hii.jpeg">Online Course: C++ Programming</a></p>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h2>Contact</h2>
    <p>Email: <a href="mailto:shahabas15kp@gmail.com">shahabas15kp@gmail.com</a></p>
    <p>Phone: +91 7306527791</p>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2025 Shahabas Ahammed K P | Srinivas University
  </footer>

</body>
</html>
