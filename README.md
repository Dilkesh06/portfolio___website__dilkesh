# portfolio___website__dilkesh
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Dilkesh | Developer Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary-color: #38bdf8;
      --secondary-color: #0f172a;
      --accent-color: #1e293b;
      --highlight-color: #a78bfa;
      --text-light: #f8fafc;
      --text-muted: #94a3b8;
      --box-color: #1e293b;
    }

    body[data-theme='green'] {
      --primary-color: #4ade80;
      --highlight-color: #bbf7d0;
    }

    body[data-theme='purple'] {
      --primary-color: #a78bfa;
      --highlight-color: #ddd6fe;
    }

    body[data-theme='red'] {
      --primary-color: #f87171;
      --highlight-color: #fecaca;
    }
    body[data-theme='light'] {
  --primary-color: #2563eb;
  --secondary-color: #ffffff;
  --accent-color: #f1f5f9;
  --highlight-color: #dbeaff;
  --text-light: #1e293b;
  --text-muted: #64748b;
  --box-color: #e2e8f3;
}

body[data-theme='dark'] {
  --primary-color: #38bdf8;
  --secondary-color: #0f172a;
  --accent-color: #1e293b;
  --highlight-color: #a78bfa;
  --text-light: #f8fafc;
  --text-muted: #94a3b8;
  --box-color: #1e293b;
}


    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background-color: var(--secondary-color);
      color: var(--text-light);
      scroll-behavior: smooth;
    }

    nav {
      background-color: var(--accent-color);
      display: flex;
      justify-content: space-between;
      padding: 20px 60px;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 999;
    }

    nav .left {
      font-size: 1.8rem;
      font-weight: bold;
      color: var(--primary-color);
      padding-left: 40px;
    }

    nav ul {
      display: flex;
      gap: 30px;
      list-style: none;
    }

    nav ul li a {
      text-decoration: none;
      color: white;
      font-weight: 500;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: var(--primary-color);
    }

    .firstSection {
      display: flex;
      justify-content: space-around;
      align-items: center;
      padding: 100px 40px;
      flex-wrap: wrap;
      background-color: #010021;
    }

    .leftSection {
      max-width: 500px;
      font-size: 2.5rem;
    }

    .leftSection span.purple {
      color: var(--highlight-color);
    }

    .leftSection .buttons {
      margin-top: 40px;
    }

    .leftSection .btn {
      padding: 12px 24px;
      background-color: var(--primary-color);
      color: var(--secondary-color);
      border: none;
      font-size: 1rem;
      font-weight: bold;
      border-radius: 8px;
      margin-right: 20px;
      cursor: pointer;
      transition: background 0.3s;
    }

    .leftSection .btn:hover {
      background-color: var(--highlight-color);
    }

    .rightSection img {
      width: 656px;
      height: 342px;
      padding-left: 300px;
      border-radius: 16px;
      animation: float 3s ease-in-out infinite;
    }

    @keyframes float {
      0% { transform: translateY(0px); }
      50% { transform: translateY(-15px); }
      100% { transform: translateY(0px); }
    }

    .secondSection {
      max-width: 90%;
      margin: auto;
      padding: 60px 20px;
    }

    .secondSection h1 {
      font-size: 2rem;
      text-align: center;
      margin-bottom: 40px;
      color: var(--primary-color);
    }

    .box {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 40px;
      justify-items: center;
    }

    .vertical {
      background: var(--box-color);
      padding: 20px;
      border-radius: 12px;
      text-align: center;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
      transition: transform 0.3s;
    }

    .vertical:hover {
      transform: translateY(-10px);
    }

    .image-top {
      width: 50px;
      margin-bottom: 15px;
    }

    .vertical-title {
      font-size: 1.1rem;
      font-weight: bold;
      margin-bottom: 8px;
    }

    .vertical-desc {
      font-size: 0.85rem;
      color: #cbd5e1;
    }

    .section-contact {
      padding: 80px 20px;
      background-color: var(--accent-color);
      color: var(--text-light);
    }

    .section-contact .container {
      max-width: 800px;
      margin: auto;
    }

    .section-contact h2 {
      text-align: center;
      color: var(--primary-color);
      font-size: 2rem;
      margin-bottom: 40px;
    }

    .contact-content {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
      margin-bottom: 30px;
    }

    .section-contact label {
      display: block;
      margin-bottom: 8px;
      font-weight: 500;
    }

    .section-contact input,
    .section-contact textarea {
      width: 100%;
      padding: 12px;
      border-radius: 8px;
      border: none;
      font-family: 'Poppins', sans-serif;
      font-size: 1rem;
      background-color: var(--secondary-color);
      color: var(--text-light);
      box-shadow: 0 0 5px rgba(56, 189, 248, 0.2);
      transition: 0.3s;
    }

    .section-contact textarea {
      resize: vertical;
    }

    .section-contact .mb-3 {
      margin-bottom: 30px;
    }

    .section-contact button {
      padding: 12px 24px;
      background-color: var(--primary-color);
      border: none;
      color: var(--secondary-color);
      font-weight: bold;
      font-size: 1rem;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    .section-contact button:hover {
      background-color: var(--highlight-color);
    }

    .footer {
      background-color: var(--secondary-color);
      padding: 60px 20px 20px;
      color: #cbd5e1;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      gap: 30px;
      max-width: 1100px;
      margin: auto;
    }

    .footer div h3 {
      margin-bottom: 10px;
      color: var(--primary-color);
    }

    .footer ul {
      list-style: none;
    }

    .footer ul li {
      margin-bottom: 8px;
      cursor: pointer;
    }

    .text-right {
      text-align: center;
      margin-top: 40px;
      font-size: 0.85rem;
      color: var(--text-muted);
    }

    .sidebar {
      position: fixed;
      top: 23px;
      left: -250px;
      height: 100vh;
      width: 250px;
      background-color: var(--accent-color);
      padding: 60px 20px;
      box-shadow: 2px 0 8px rgba(0,0,0,0.2);
      transition: left 0.3s ease;
      z-index: 999;
    }

    .sidebar.active {
      left: 0;
    }

    .sidebar h2 {
      color: var(--primary-color);
      margin-bottom: 30px;
      font-size: 2.5rem;
    }

    .sidebar ul {
      list-style: none;
      padding: 0;
    }

    .sidebar ul li {
      margin: 20px 0;
    }

    .sidebar ul li a {
      color: var(--text-light);
      text-decoration: none;
      font-size: 1rem;
      font-weight: 500;
    }

    #themeSwitcher {
      position: fixed;
      top: 20px;
      right: 10px;
      z-index: 1000;
      padding: 8px;
      border-radius: 6px;
      background: var(--primary-color);
      color: var(--secondary-color);
      font-weight: bold;
      border: none;
      cursor: pointer;
    }

    @media(max-width: 768px) {
      nav {
        flex-direction: column;
        gap: 10px;
      }
      nav ul {
        flex-direction: column;
        gap: 10px;
      }
      .rightSection img {
        padding-left: 0;
      }
    }
  </style>
</head>
<body data-theme="default">

<!-- Theme Switcher -->
<select id="themeSwitcher">
  <option value="default">Blue Theme</option>
  <option value="light">Light Theme</option>
     <option value="dark">Dark Theme</option>
  <option value="green">Green Theme</option>
  <option value="purple">Purple Theme</option>
  <option value="red">Red Theme</option>
</select>

<!-- Sidebar Toggle -->
<button id="sidebarToggle" style="position: fixed; top: 20px; left: 20px; z-index: 1000; background: var(--primary-color); border: none; padding: 10px 15px; border-radius: 8px; cursor: pointer;">
  ☰
</button>

<!-- Sidebar -->
<div id="sidebar" class="sidebar">
  <h2>Menu</h2>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Sign In</a></li>
    <li><a href="#">Settings</a></li>
    <li><a href="#">Help</a></li>
    <li><a href="#">Feedback</a></li>
  </ul>
</div>

<!-- Navbar -->
<nav>
  <div class="left">Dilkesh</div>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Services</a></li>
    <li><a href="#">Projects</a></li>
    <li><a href="#actual-contact">Contact</a></li>
  </ul>
</nav>

<!-- Hero -->
<section class="firstSection">
  <div class="leftSection">
    Hi, My name is <span class="purple">Dilkesh</span>
    <div>and I am a passionate Web Developer</div>
    <span id="element"></span>
    <div class="buttons">
      <a href="realAmazonclone.html"><button class="btn">My Amazon Clone</button></a>
      <a href="#actual-contact"><button class="btn">Contact Me</button></a>
    </div>
  </div>
  <div class="rightSection">
    <img src="p1.png" alt="Dilkesh Image">
  </div>
</section>

<!-- Work Section -->
<section class="secondSection">
  <h1>My Work Experience</h1>
  <div class="box">
    <div class="vertical"><img class="image-top" src="videogame.jpg"><div class="vertical-title">HTML Developer</div><div class="vertical-desc">Built responsive layouts and animated interfaces.</div></div>
    <div class="vertical"><img class="image-top" src="facebooklogo.png"><div class="vertical-title">Node.js - Facebook</div><div class="vertical-desc">Worked on GraphQL APIs & backend microservices.</div></div>
    <div class="vertical"><img class="image-top" src="twiterlogo.png"><div class="vertical-title">Frontend - Twitter</div><div class="vertical-desc">Optimized widgets and timeline performance.</div></div>
    <div class="vertical"><img class="image-top" src="githublogo.png"><div class="vertical-title">Open Source - GitHub</div><div class="vertical-desc">Maintained and contributed React components.</div></div>
  </div>
</section>

<!-- Contact Section -->
<section class="section-contact" id="actual-contact">
  <div class="container">
    <h2>Contact Me</h2>
    <form
  action="https://formspree.io/f/xvgaqyvn"
  method="POST"
>
      <div class="contact-content">
        <div>
          <label for="username">Name</label>
          <input type="text" name="username" placeholder="Enter your name" required />
        </div>
        <div>
          <label for="email">Email</label>
          <input type="email" name="email" placeholder="Enter your email" required />
        </div>
      </div>
      <div class="mb-3">
        <label for="message">Message</label>
        <textarea name="message" rows="5" placeholder="Your message here..." required></textarea>
      </div>
      <button type="submit">Send Message</button>
    </form>
  </div>
</section>

<!-- Map -->
<div class="map">
  <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3491.188059584499!2d77.10134887410887!3d28.952146069497505!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x390dadd1ccaa6249%3A0x79dedc8ba40cf3ac!2sIndian%20Institute%20Of%20Information%20Technology%20Sonepat!5e0!3m2!1sen!2sin!4v1745905721856!5m2!1sen!2sin" width="100%" height="500" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
</div>

<!-- Footer -->
<footer>
  <div class="footer">
    <div><h3>Quick Links</h3><ul><li>Home</li><li>About</li><li>Projects</li></ul></div>
    <div><h3>Connect</h3><ul><li>LinkedIn</li><li>GitHub</li><li>Twitter</li></ul></div>
    <div><h3>Resources</h3><ul><li>Resume</li><li>Skills</li><li>Certificates</li></ul></div>
  </div>
  <div class="text-right">© 2025 Dilkesh's Portfolio. All rights reserved.</div>
</footer>

<!-- Scripts -->
<script src="https://unpkg.com/typed.js@2.1.0/dist/typed.umd.js"></script>
<script>
  new Typed('#element', {
    strings: ['Web Developer.', 'Video Designer.', 'Creative Coder.', 'UI Designer.'],
    typeSpeed: 60,
    backSpeed: 40,
    loop: true,
  });

  document.getElementById('sidebarToggle').addEventListener('click', () => {
    document.getElementById('sidebar').classList.toggle('active');
  });

  document.getElementById('themeSwitcher').addEventListener('change', (e) => {
    document.body.setAttribute('data-theme', e.target.value);
  });
</script>

</body>
</html>
