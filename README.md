##index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Disha H Thakur Portfolio</title>
  <link rel="stylesheet" href="styles.css" />
  <script defer src="script.js"></script>
</head>
<body>
  <header>
    <nav class="navbar">
      <div class="logo">Disha H Thakur</div>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#achievements">Achievements</a></li>
        <li><a href="#resume">Resume</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
      <button class="theme-toggle" id="themeToggle">🌙</button>
    </nav>
  </header>

  <main>
    <!-- HOME -->
    <section id="home" class="section">
      <img src="https://drive.google.com/uc?export=view&id=1bIYbUumkKQg35-uR87iGTPP97823m9Aa" alt="Profile Photo" class="profile-img">
      <h1>Hello, I’m <span class="highlight">Disha H Thakur</span></h1>
      <p class="tagline">Aspiring Tech Enthusiast | Lifelong Learner | Future-Ready Engineer</p>
    </section>

    <!-- ABOUT -->
    <section id="about" class="section">
      <h2>About Me</h2>
      <p>
        I’m currently pursuing my Bachelor's degree in Computer Engineering at the Government College of Engineering, Nagpur. I’m passionate about technology, coding, and problem-solving. My goal is to become a future-ready engineer contributing to impactful tech solutions.
      </p>
      <ul class="values">
        <li>Innovation</li>
        <li>Continuous Learning</li>
        <li>Collaboration</li>
      </ul>
    </section>

    <!-- SKILLS -->
    <section id="skills" class="section">
      <h2>Skills</h2>
      <div class="skills-container">
        <span class="skill">C</span>
        <span class="skill">Python</span>
        <span class="skill">Java</span>
        <span class="skill">HTML</span>
        <span class="skill">CSS</span>
        <span class="skill">JavaScript</span>
        <span class="skill">Communication</span>
        <span class="skill">Leadership</span>
      </div>
    </section>

    <!-- PROJECTS -->
    <section id="projects" class="section">
      <h2>Projects</h2>
      <div class="project-card">
        <h3>Weather App</h3>
        <p>A web app showing real-time weather info using OpenWeatherMap API.</p>
        <p class="tools">Tools: HTML, CSS, JS</p>
        <a href="https://github.com/Disha220205" target="_blank" class="btn">GitHub</a>
      </div>
      <div class="project-card">
        <h3>Student Management System</h3>
        <p>Desktop app to manage student records efficiently.</p>
        <p class="tools">Tools: Java, MySQL</p>
      </div>
      <div class="project-card">
        <h3>Portfolio Website</h3>
        <p>This portfolio site built with HTML, CSS, JS.</p>
        <p class="tools">Tools: HTML, CSS, JS</p>
      </div>
    </section>

    <!-- ACHIEVEMENTS -->
    <section id="achievements" class="section">
      <h2>Achievements & Certifications</h2>
      <ul>
        <li>Winner, Hackathon 2024 - College Level</li>
        <li>Completed Python for Everybody - Coursera</li>
        <li>3rd place in Code Challenge 2023</li>
      </ul>
    </section>

    <!-- RESUME -->
    <section id="resume" class="section">
      <h2>Resume</h2>
      <img src="https://drive.google.com/uc?export=view&id=18K5arbjxRBtXkiFSOfwD8YKUsWQHW6U5" alt="Resume Preview" class="resume-preview"/>
      <br/>
      <a href="https://drive.google.com/file/d/18K5arbjxRBtXkiFSOfwD8YKUsWQHW6U5/view?usp=drivesdk" target="_blank" class="btn">Download Resume</a>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="section">
      <h2>Contact</h2>
      <form id="contactForm">
        <input type="text" placeholder="Your Name" required />
        <input type="email" placeholder="Your Email" required />
        <textarea placeholder="Your Message" required></textarea>
        <button type="submit" class="btn">Send</button>
      </form>
      <div class="socials">
        <a href="https://www.linkedin.com/in/disha-h-thakur" target="_blank">LinkedIn</a>
        <a href="mailto:disha@example.com">Email</a>
        <a href="https://github.com/Disha220205" target="_blank">GitHub</a>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Disha H Thakur</p>
  </footer>
</body>
</html>

##style.css
*
{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: "Segoe UI", sans-serif;
  background: #fff;
  color: #333;
  line-height: 1.6;
}

.dark {
  background: #121212;
  color: #ddd;
}

header {
  position: sticky;
  top: 0;
  background: #fff;
  z-index: 1000;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.dark header {
  background: #1e1e1e;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1em;
  max-width: 1200px;
  margin: auto;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1em;
  flex-wrap: wrap;
}

.nav-links a {
  text-decoration: none;
  color: inherit;
  font-weight: bold;
}

.theme-toggle {
  background: none;
  border: none;
  font-size: 1.2em;
  cursor: pointer;
}

.section {
  padding: 60px 20px;
  max-width: 1000px;
  margin: auto;
  opacity: 0;
  transform: translateY(30px);
  transition: all 0.8s ease-out;
}

.section.visible {
  opacity: 1;
  transform: translateY(0);
}

h2 {
  margin-bottom: 1em;
  font-size: 2em;
  color: #007acc;
}

.highlight {
  color: #007acc;
}

.profile-img {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 1em;
  box-shadow: 0 4px 15px rgba(0,0,0,0.2);
}

.tagline {
  font-size: 1.2em;
  margin-top: 0.5em;
}

.values {
  display: flex;
  gap: 1em;
  list-style: none;
  margin-top: 1em;
}

.values li {
  background: #007acc;
  color: #fff;
  padding: 0.5em 1em;
  border-radius: 20px;
}

.skills-container {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.skill {
  background: #007acc;
  color: #fff;
  padding: 8px 16px;
  border-radius: 20px;
  font-size: 0.9em;
}

.project-card {
  background: #f7f7f7;
  margin: 1em 0;
  padding: 1em;
  border-radius: 8px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}

.dark .project-card {
  background: #1e1e1e;
  color: #ddd;
}

.tools {
  font-style: italic;
  font-size: 0.9em;
  margin-top: 0.5em;
}

.btn {
  display: inline-block;
  background: #007acc;
  color: #fff;
  padding: 0.5em 1em;
  text-decoration: none;
  border-radius: 4px;
  margin-top: 0.5em;
}

.btn:hover {
  background: #005fa3;
}

.resume-preview {
  width: 100%;
  max-width: 400px;
  margin: 1em 0;
}

form {
  display: flex;
  flex-direction: column;
  gap: 10px;
  max-width: 500px;
}

form input,
form textarea {
  padding: 0.8em;
  border: 1px solid #ccc;
  border-radius: 4px;
  font: inherit;
}

form button {
  cursor: pointer;
}

.socials {
  margin-top: 20px;
}

.socials a {
  margin-right: 1em;
  color: #007acc;
  text-decoration: none;
}

footer {
  text-align: center;
  padding: 2em;
  font-size: 0.9em;
  color: #888;
}

##script.js
// Dark mode toggle
const toggleBtn = document.getElementById("themeToggle");
toggleBtn.addEventListener("click", () => {
  document.body.classList.toggle("dark");
  toggleBtn.textContent = document.body.classList.contains("dark") ? "☀️" : "🌙";
});

// Scroll animations
const sections = document.querySelectorAll(".section");
window.addEventListener("scroll", () => {
  const triggerBottom = window.innerHeight * 0.8;
  sections.forEach((sec) => {
    const rect = sec.getBoundingClientRect();
    if (rect.top < triggerBottom) {
      sec.classList.add("visible");
    }
  });
});

// Contact form submit (dummy)
document.getElementById("contactForm").addEventListener("submit", (e) => {
  e.preventDefault();
  alert("Thank you! Your message has been sent.");
  e.target.reset();
});
