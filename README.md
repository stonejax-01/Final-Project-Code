<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Jackson's Cloud Computing Final Project</title>
  <link rel="stylesheet" href="CloudComputingStyle.css" />
</head>
<body>
  <nav>
    <div class="logo">Welcome To My Site</div>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#cloud">Cloud Project</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <header>
    <h1>Welcome to My Cloud Computing Final Website</h1>
    <p>Hosted on AWS S3 | Built with HTML5, CSS3, and ✨magic (AKA code, anger and tons of focus)✨</p>
  </header>

  <main>
    <section id="about">
      <h2>About Me</h2>
      <p>I'm a soon-to-be graduate with skills in UX/UI design, HTML/CSS, and cloud computing using AWS. This site is part of my final to show how I can host a static site using AWS. (Pretty Cool Right?)</p>
    </section>

    <section id="skills">
      <h2>College Skills</h2>
      <ul class="skills-grid">
        <li>HTML5 + CSS3</li>
        <li>AWS S3 Static Hosting</li>
        <li>UI Prototyping</li>
        <li>Responsive Design</li>
        <li>Git + GitHub</li>
        <li>Premiere Pro</li>
        <li>Photoshop Portfolio</li>
        <li>YT Channel</li>
      </ul>
    </section>

    <section id="cloud">
      <h2>About This Project</h2>
      <p>This project is hosted on an AWS S3 bucket and demonstrates the power of static site hosting in the cloud. It's fast, scalable, and affordable for simple sites like portfolios or Resumes. And I purchased a domain name to top it all off.</p>
      
      <div class="video-wrapper">
        <iframe src="https://www.youtube.com/embed/EIeh2A4XxeE?si=JIv2LEtsaVch6ROO" title="YouTube video" allowfullscreen></iframe>
      </div>
    </section>

    <section id="contact">
      <h2>Contact Me</h2>
      <p>Want to collab, hire me, or just say hey? Reach out: <a href="mailto:pingeljackson@gmail.com">Pingeljackson@gmail.com</a></p>
    </section>
  </main>

  <footer>
    <p>© 2025 Jackson Pingel | Cloud Final Project | Made with love + caffeine + procrastination</p>
  </footer>
</body>
</html>
/* Reset + Base */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Segoe UI', sans-serif;
  background: #f9fafb;
  color: #111827;
  line-height: 1.6;
  padding-top: 4rem;
  animation: fadeIn 1s ease-in;
}

/* Nav bar */
nav {
  background: #1f2937;
  color: white;
  padding: 1rem 2rem;
  position: fixed;
  width: 100%;
  top: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 1000;
}

nav .logo {
  font-size: 1.5rem;
  font-weight: bold;
}

nav ul {
  display: flex;
  gap: 1.5rem;
  list-style: none;
}

nav ul li a {
  color: white;
  text-decoration: none;
  font-weight: 500;
}

nav ul li a:hover {
  text-decoration: underline;
}

/* Header */
header {
  background: #4f46e5;
  color: white;
  padding: 3rem 2rem;
  text-align: center;
  margin-top: 1rem;
  border-radius: 12px;
  animation: slideIn 0.8s ease-in-out;
}

main {
  max-width: 1000px;
  margin: auto;
  padding: 2rem;
}

section {
  margin-bottom: 3rem;
  background: white;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
  animation: fadeInUp 0.8s ease;
}

/* Skills Grid */
.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 1rem;
  list-style: none;
  padding: 0;
}

.skills-grid li {
  background: #e5e7eb;
  padding: 1rem;
  text-align: center;
  border-radius: 8px;
  font-weight: bold;
  transition: all 0.3s ease;
  cursor: pointer;
}

.skills-grid li:hover {
  background: #4f46e5;
  color: white;
  transform: scale(1.05);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
}

/* Responsive YouTube Embed */
.video-wrapper {
  position: relative;
  padding-bottom: 56.25%;
  height: 0;
  overflow: hidden;
  border-radius: 12px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
  margin: 2rem 0;
}

.video-wrapper iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
  border-radius: 12px;
}

/* Footer */
footer {
  text-align: center;
  padding: 2rem;
  color: #6b7280;
}

/* Animations */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes slideIn {
  from { transform: translateY(-20px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

@keyframes fadeInUp {
  from { transform: translateY(30px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}
