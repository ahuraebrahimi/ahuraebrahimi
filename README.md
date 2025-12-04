<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ahura Code - Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;700&family=Roboto:wght@400;700&display=swap" rel="stylesheet">
<style>
  :root {
    --primary-color: #8A2BE2;
    --secondary-color: #A778FF;
    --bg-color: #1a1a1a;
    --text-color: #fff;
    --card-bg: #222;
  }
  * {margin:0; padding:0; box-sizing:border-box; font-family: 'Roboto', sans-serif;}
  body {background: var(--bg-color); color: var(--text-color);}
  a {color: inherit; text-decoration: none;}
  img {max-width:100%; display:block;}

  /* ===== Scroll to Top Button ===== */
  #scrollTop {
    position: fixed;
    bottom: 30px;
    right: 30px;
    background: var(--primary-color);
    color: #fff;
    border:none;
    padding:12px 16px;
    border-radius:50%;
    font-size:20px;
    cursor:pointer;
    display:none;
    z-index:100;
    box-shadow:0 4px 10px rgba(0,0,0,0.3);
    transition: 0.3s;
  }
  #scrollTop:hover {background: var(--secondary-color);}

  /* ===== Header ===== */
  header {
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    background: linear-gradient(135deg, #8A2BE2, #A778FF);
  }
  header img {width:180px; border-radius:50%; box-shadow:0 0 35px #a873ff;}
  header h1 {font-size:3rem; margin-top:20px;}
  .typed-text {color:#fff; font-weight:700; font-size:1.5rem; margin-top:10px;}
  .header-btn {margin-top:20px; padding:12px 25px; background:#fff; color: var(--primary-color); font-weight:bold; border-radius:25px; transition:0.3s;}
  .header-btn:hover {background: var(--secondary-color); color:#fff;}

  /* ===== Sections ===== */
  section {padding:80px 20px; max-width:1200px; margin:0 auto;}
  h2 {text-align:center; font-size:2.5rem; margin-bottom:40px; color: var(--primary-color);}

  /* ===== Skills ===== */
  .skills {display:flex; flex-wrap:wrap; justify-content:center; gap:20px;}
  .skill {background: var(--card-bg); padding:20px; border-radius:15px; width:220px; box-shadow:0 4px 15px rgba(0,0,0,0.3);}
  .skill h3 {margin-bottom:10px; color:var(--secondary-color);}
  .progress-bar {height:12px; background:#333; border-radius:10px; overflow:hidden;}
  .progress {height:100%; width:0%; background: var(--primary-color); border-radius:10px;}

  /* ===== Projects ===== */
  .projects {display:flex; flex-wrap:wrap; justify-content:center; gap:25px;}
  .project-card {background: var(--card-bg); border-radius:15px; width:250px; padding:20px; text-align:center; box-shadow:0 4px 15px rgba(0,0,0,0.3); transition:0.3s;}
  .project-card:hover {transform: translateY(-10px); box-shadow:0 10px 25px rgba(0,0,0,0.5);}
  .project-card img {width:80px; margin-bottom:15px;}
  .project-card h4 {margin-bottom:10px; color: var(--secondary-color);}
  .project-card p {font-size:0.9rem; color:#ccc;}

  /* ===== Certificates ===== */
  .certificates {display:flex; flex-wrap:wrap; justify-content:center; gap:25px;}
  .certificate-card {background: var(--card-bg); border-radius:15px; width:220px; padding:15px; text-align:center; box-shadow:0 4px 15px rgba(0,0,0,0.3); transition:0.3s;}
  .certificate-card:hover {transform: translateY(-10px); box-shadow:0 10px 25px rgba(0,0,0,0.5);}
  .certificate-card img {width:60px; margin-bottom:10px;}
  .certificate-card h5 {color: var(--secondary-color); margin-bottom:5px;}
  .certificate-card p {font-size:0.85rem; color:#ccc;}

  /* ===== Contact ===== */
  .contact {text-align:center;}
  .contact a {display:inline-block; margin:10px; padding:10px 20px; background: var(--primary-color); border-radius:25px; font-weight:bold; transition:0.3s;}
  .contact a:hover {background: var(--secondary-color);}

</style>
</head>
<body>

<!-- ===== Scroll To Top Button ===== -->
<button id="scrollTop" onclick="topFunction()">↑</button>

<!-- ===== Header ===== -->
<header>
  <img src="https://github.com/USERNAME.png" alt="Ahura Ebrahimi">
  <h1>Ahura Ebrahimi</h1>
  <div class="typed-text" id="typed"></div>
  <a href="Ahura_Ebrahimi_Resume.pdf" download class="header-btn">Download Resume</a>
</header>

<!-- ===== Skills Section ===== -->
<section id="skills">
  <h2>💻 Skills</h2>
  <div class="skills">
    <div class="skill">
      <h3>Web Development</h3>
      <div class="progress-bar"><div class="progress" data-width="90%"></div></div>
    </div>
    <div class="skill">
      <h3>WordPress</h3>
      <div class="progress-bar"><div class="progress" data-width="90%"></div></div>
    </div>
    <div class="skill">
      <h3>Python</h3>
      <div class="progress-bar"><div class="progress" data-width="85%"></div></div>
    </div>
    <div class="skill">
      <h3>Game Development</h3>
      <div class="progress-bar"><div class="progress" data-width="70%"></div></div>
    </div>
    <div class="skill">
      <h3>Java</h3>
      <div class="progress-bar"><div class="progress" data-width="70%"></div></div>
    </div>
  </div>
</section>

<!-- ===== Projects Section ===== -->
<section id="projects">
  <h2>📂 Projects</h2>
  <div class="projects">
    <div class="project-card">
      <img src="https://img.icons8.com/color/96/000000/snake.png"/>
      <h4>Snake Game</h4>
      <p>Fast, smooth gameplay. Python & Pygame</p>
    </div>
    <div class="project-card">
      <img src="https://img.icons8.com/color/96/000000/rubik.png"/>
      <h4>Rubik’s Cube Solver</h4>
      <p>Mobile learning & solver app. App Inventor</p>
    </div>
    <div class="project-card">
      <img src="https://img.icons8.com/color/96/000000/cloud.png"/>
      <h4>Weather App</h4>
      <p>Beautiful API-powered UI. HTML, CSS, JS</p>
    </div>
    <div class="project-card">
      <img src="https://img.icons8.com/color/96/000000/shopping-cart.png"/>
      <h4>Shalil Store</h4>
      <p>Modern eCommerce site. WordPress</p>
    </div>
  </div>
</section>

<!-- ===== Certificates Section ===== -->
<section id="certificates">
  <h2>🎓 Certificates</h2>
  <div class="certificates">
    <div class="certificate-card">
      <img src="https://img.icons8.com/color/96/000000/harvard.png"/>
      <h5>CS50 Harvard</h5>
      <p>Harvard University</p>
    </div>
    <div class="certificate-card">
      <img src="https://img.icons8.com/color/96/000000/python.png"/>
      <h5>Python Course</h5>
      <p>Iran Digital</p>
    </div>
    <div class="certificate-card">
      <img src="https://img.icons8.com/color/96/000000/scratch.png"/>
      <h5>Scratch Game Dev</h5>
      <p>Iran Scratch Academy</p>
    </div>
    <div class="certificate-card">
      <img src="https://img.icons8.com/color/96/000000/android.png"/>
      <h5>App Inventor Dev</h5>
      <p>Iran Scratch Academy</p>
    </div>
    <div class="certificate-card">
      <img src="https://img.icons8.com/color/96/000000/game-controller.png"/>
      <h5>Game Maker Dev</h5>
      <p>Iran Scratch Academy</p>
    </div>
    <div class="certificate-card">
      <img src="https://img.icons8.com/color/96/000000/star.png"/>
      <h5>Front-End Web Dev</h5>
      <p>Starcoach</p>
    </div>
  </div>
</section>

<!-- ===== Contact Section ===== -->
<section id="contact">
  <h2>📞 Contact</h2>
  <div class="contact">
    <a href="mailto:ahuracodes@gmail.com">Email Me</a>
    <a href="tel:+989046855918">Call Me</a>
    <a href="https://linkedin.com/in/ahura-ebrahimi-923948383" target="_blank">LinkedIn</a>
    <a href="https://www.ahuracode.ir" target="_blank">Website</a>
  </div>
</section>

<script>
  // ===== Typed Text =====
  const typedText = document.getElementById('typed');
  const phrases = ["Full-Stack Developer", "Python / Java", "Web / Mobile / Game Dev", "Turning Ideas into Code"];
  let i = 0, j = 0, currentPhrase = [], isDeleting=false;
  function type(){
    if(i >= phrases.length) i=0;
    let fullPhrase = phrases[i];
    if(!isDeleting) {
      currentPhrase.push(fullPhrase[j]);
      typedText.textContent = currentPhrase.join('');
      j++;
      if(j === fullPhrase.length){isDeleting=true; setTimeout(type,1000);} else {setTimeout(type,100);}
    } else {
      currentPhrase.pop();
      typedText.textContent = currentPhrase.join('');
      if(currentPhrase.length===0){isDeleting=false; j=0; i++; setTimeout(type,200);} else {setTimeout(type,50);}
    }
  }
  type();

  // ===== Progress Bars Animation =====
  const progressBars = document.querySelectorAll('.progress');
  window.addEventListener('scroll',()=>{
    progressBars.forEach(bar=>{
      let value = bar.getAttribute('data-width');
      let barPos = bar.getBoundingClientRect().top;
      let screenPos = window.innerHeight/1.2;
      if(barPos < screenPos) {bar.style.width = value;}
    });
  });

  // ===== Scroll to Top Button =====
  const scrollBtn = document.getElementById("scrollTop");
  window.onscroll = function() {
    if (document.body.scrollTop > 300 || document.documentElement.scrollTop > 300) {
      scrollBtn.style.display = "block";
    } else {scrollBtn.style.display = "none";}
  };
  function topFunction(){window.scrollTo({top:0,behavior:'smooth'});}
</script>

</body>
</html>
