<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Portfolio</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet" />
  <link rel="icon" href="favicon.ico" />
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      padding: 0;
      background: #2f2525;
      color: #fcfcfc;
    }
    nav {
      background: #ff0000;
      padding: 15px;
      text-align: center;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #000;
    }
    .container {
      padding: 20px;
      text-align: center;
    }
    .tab {
      display: none;
      background: #222;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);
      max-width: 700px;
      margin: 40px auto;
    }
    .tab.active {
      display: block;
    }
    h1 {
      color: #ff0000;
      font-size: 2em;
    }
    p {
      font-size: 1.2em;
    }
    img, video {
      max-width: 100%;
      border-radius: 10px;
      margin-top: 20px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
    }
    button {
      background: #6a0dad;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background 0.3s;
    }
    button:hover {
      background: #d4a5ff;
    }
    a.project-link {
      color: #00ff88;
    }
  </style>
  <script>
    function showTab(tabId) {
      document.querySelectorAll('.tab').forEach(tab => tab.classList.remove('active'));
      document.getElementById(tabId).classList.add('active');
    }
  </script>
</head>
<body>
  <nav>
    <a href="#" onclick="showTab('home')">Home</a>
    <a href="#" onclick="showTab('about')">About</a>
    <a href="#" onclick="showTab('projects')">Projects</a>
    <a href="#" onclick="showTab('certificates')">Certificates</a>
    <a href="#" onclick="showTab('contact')">Contact</a>
    <a href="#" onclick="showTab('resume')">Resume</a>
  </nav>

  <div class="container">
    <div id="home" class="tab active">
      <h1>Welcome to My Portfolio</h1>
      <p>Explore my work and skills.</p>
      <img src="your-image.jpg" alt="Portfolio banner or logo" />
    </div>

    <div id="about" class="tab">
      <h1>About Me</h1>
      <p>
        Hi! I'm a beginner front-end web developer who enjoys building creative and responsive websites.
        My journey started in college during an Electromechanical Manufacturing Lab class I didn’t enjoy. I discovered 
        <a href="https://www.freecodecamp.org" target="_blank" class="project-link">freeCodeCamp</a> and started learning!
      </p>
      <p>
        Some fun projects I’ve built:
        <br>• <a href="https://www.freecodecamp.org/learn/2022/responsive-web-design/learn-html-by-building-a-cat-photo-app/step-71" 
                 target="_blank" class="project-link">Cat Photo App</a><br>
        • <a href="https://www.freecodecamp.org/learn/2022/responsive-web-design/learn-basic-css-by-building-a-cafe-menu/step-91" 
             target="_blank" class="project-link">Café Menu</a>
      </p>
      <p>
        These helped me build a solid foundation in HTML and CSS, and I’m now working toward becoming a full-fledged front-end developer.
      </p>
      <img src="https://media.discordapp.net/attachments/1071241512295354479/1369685128036614405/IMG_1383.png" 
           alt="Photo of me" style="width: 250px; height: 250px; object-fit: cover;" />
    </div>

    <div id="projects" class="tab">
      <h1>My Projects</h1>
      <p>A showcase of my work.</p>
      <img src="project-image.jpg" alt="Screenshot of project" />
      <video controls>
        <source src="project-demo.mp4" type="video/mp4" />
        Your browser does not support the video tag.
      </video>
    </div>

    <div id="certificates" class="tab">
      <h1>My Certificates</h1>
      <p>Here are some of the certificates I’ve earned:</p>
      <img src="certificate1.jpg" alt="Certificate 1" />
      <img src="certificate2.jpg" alt="Certificate 2" />
    </div>

    <div id="contact" class="tab">
      <h1>Contact Me</h1>
      <p>Get in touch with me here.</p>
      <img src="contact-image.jpg" alt="Contact illustration" />
      <br /><br />
      <button onclick="window.location.href='mailto:your-email@example.com'">Email Me</button>
    </div>

    <div id="resume" class="tab">
      <h1>Resume</h1>
      <p>Here's my resume:</p>
      <img src="assets/images/resume-img.jpg" alt="Screenshot of resume" />
      <br /><br />
      <button onclick="window.open('https://docs.google.com/document/d/1O3HGr_Bz3lpOl4b6u-m5nZuhN2RrXvQPUI-UjIYauhY/edit?usp=sharing', '_blank')">View Resume</button>
    </div>
  </div>
</body>
</html>

