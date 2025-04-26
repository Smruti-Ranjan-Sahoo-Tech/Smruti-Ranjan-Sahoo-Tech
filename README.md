<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Smruti Ranjan Sahoo | Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      padding: 0;
      background-color: var(--bg-color);
      color: var(--text-color);
      transition: background-color 0.3s, color 0.3s;
    }
    :root {
      --bg-color: #ffffff;
      --text-color: #000000;
    }
    [data-theme="dark"] {
      --bg-color: #1e1e1e;
      --text-color: #ffffff;
    }
    .container {
      padding: 2rem;
      max-width: 1200px;
      margin: auto;
    }
    .toggle-switch {
      position: fixed;
      top: 20px;
      right: 20px;
      display: flex;
      align-items: center;
      gap: 10px;
      cursor: pointer;
    }
    .switch {
      position: relative;
      display: inline-block;
      width: 60px;
      height: 34px;
    }
    .switch input {
      opacity: 0;
      width: 0;
      height: 0;
    }
    .slider {
      position: absolute;
      cursor: pointer;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background-color: #ccc;
      transition: .4s;
      border-radius: 34px;
    }
    .slider:before {
      position: absolute;
      content: "";
      height: 26px;
      width: 26px;
      left: 4px;
      bottom: 4px;
      background-color: white;
      transition: .4s;
      border-radius: 50%;
    }
    input:checked + .slider {
      background-color: #2196F3;
    }
    input:checked + .slider:before {
      transform: translateX(26px);
    }
    .skills img {
      margin: 10px;
      width: 50px;
      height: 50px;
      transition: transform 0.3s;
    }
    .skills img:hover {
      transform: scale(1.2);
    }
    h1, h2, p {
      text-align: center;
    }
    .center-img {
      display: flex;
      justify-content: center;
      margin: 20px 0;
    }
    footer {
      text-align: center;
      padding: 2rem 0;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>

<div class="toggle-switch">
  <label class="switch">
    <input type="checkbox" id="theme-toggle">
    <span class="slider"></span>
  </label>
  <span id="mode-icon">🌞</span>
</div>

<div class="container">
  <h1>Hi 👋, I'm Smruti Ranjan Sahoo</h1>
  <h2>A passionate Frontend Developer from India</h2>

  <div class="center-img">
    <img src="https://cdn.dribbble.com/users/1162077/screenshots/3848914/programmer.gif" alt="Coding" width="400">
  </div>

  <p>🔭 I’m currently working on Fun Projects like Games and Websites</p>
  <p>🌱 I’m currently learning Advanced JavaScript, React, and Backend Development</p>
  <p>👯 I’m looking to collaborate on Open Source Projects</p>
  <p>💬 Ask me about Frontend Development, JavaScript, and Web Design</p>
  <p>📫 How to reach me: <strong>s.r.sahoo370@gmail.com</strong></p>
  <p>⚡ Fun fact: I love solving real-world problems with simple code!</p>

  <h2>🛠️ Languages and Tools</h2>
  <div class="skills center-img">
    <a href="https://developer.mozilla.org/en-US/docs/Web/HTML" target="_blank">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="HTML5">
    </a>
    <a href="https://developer.mozilla.org/en-US/docs/Web/CSS" target="_blank">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="CSS3">
    </a>
    <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript">
    </a>
    <a href="https://getbootstrap.com/" target="_blank">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="Bootstrap">
    </a>
  </div>

  <h2>📈 GitHub Stats</h2>
  <div class="center-img">
    <img src="https://github-readme-stats.vercel.app/api?username=Smruti-Ranjan-Sahoo-Tech&show_icons=true&locale=en" alt="GitHub Stats">
  </div>

  <h2>🏆 GitHub Trophies</h2>
  <div class="center-img">
    <img src="https://github-profile-trophy.vercel.app/?username=Smruti-Ranjan-Sahoo-Tech" alt="GitHub Trophies">
  </div>

  <h2>✍️ Random Developer Quote</h2>
  <div class="center-img">
    <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=light" alt="Dev Quote">
  </div>

</div>

<footer>
  <p>Made with ❤️ by Smruti Ranjan Sahoo</p>
</footer>

<script>
const themeToggle = document.getElementById('theme-toggle');
const modeIcon = document.getElementById('mode-icon');

function setTheme(mode) {
  if (mode === 'dark') {
    document.documentElement.setAttribute('data-theme', 'dark');
    modeIcon.textContent = '🌑';
  } else {
    document.documentElement.removeAttribute('data-theme');
    modeIcon.textContent = '🌞';
  }
}

themeToggle.addEventListener('change', () => {
  if (themeToggle.checked) {
    setTheme('dark');
  } else {
    setTheme('light');
  }
});
</script>

</body>
</html>
