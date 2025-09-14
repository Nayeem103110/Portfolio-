<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Shaik NayeeM'S Portfolio</title>
  <style>
  :root{
    --accent:#22c55e;   /* green */
    --muted:#9ca3af;
    --card:#111827;     /* dark gray for cards */
    --bg:#000000;       /* black background */
    --hover:#16a34a;    /* bright green hover */
    --highlight:#4ade80;/* light green highlight */
  }

  *{box-sizing:border-box;}

  body{
    font-family:Inter,ui-sans-serif,system-ui,Helvetica,Arial;
    color:#f9fafb;
    background:var(--bg);
    margin:0;
    line-height:1.45;
    transition: background 0.5s ease, color 0.5s ease;
  }

  .container{max-width:980px;margin:28px auto;padding:24px}

  header{display:flex;align-items:center;justify-content:space-between;gap:18px;transition: all 0.3s ease;}
  header:hover{transform: scale(1.01);}

  .brand{display:flex;align-items:center;gap:14px}

  .avatar{
    width:72px;
    height:72px;
    border-radius:50%;
    background:linear-gradient(135deg,var(--accent),var(--highlight));
    color:#fff;
    display:grid;
    place-items:center;
    font-weight:700;
    font-size:20px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .avatar:hover{
    transform: scale(1.1);
    box-shadow: 0 0 18px rgba(34,197,94,0.6);
  }

  h1{margin:0;font-size:22px; color: var(--accent);}
  p.lead{color:var(--muted);margin:6px 0 0; transition: color 0.3s ease;}

  .actions{display:flex;gap:10px;}
  .btn{
    display:inline-block;
    padding:8px 12px;
    border-radius:8px;
    text-decoration:none;
    font-weight:600;
    transition: all 0.3s ease;
    cursor:pointer;
    border:none;
  }
  .btn-primary{
    background:var(--accent);
    color:#000;
  }
  .btn-primary:hover{
    background:var(--hover);
    transform: translateY(-2px);
    box-shadow: 0 6px 12px rgba(34,197,94,0.3);
    color:#fff;
  }

  .tab-section{display:none; transition: all 0.5s ease;}

  .card{
    background:var(--card);
    padding:16px;
    border-radius:12px;
    box-shadow:0 6px 18px rgba(0,0,0,0.6);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .card:hover{
    transform: translateY(-4px);
    box-shadow: 0 10px 24px rgba(0,0,0,0.9);
  }

  .projects{display:grid;gap:12px}
  .project{display:flex;gap:12px;align-items:flex-start}
  .thumb{
    width:120px;
    height:78px;
    border-radius:8px;
    background: linear-gradient(135deg,#064e3b,#22c55e);
    display:grid;
    place-items:center;
    color:#fff;
    font-weight:700;
    transition: transform 0.3s ease, background 0.3s ease;
  }
  .thumb:hover{
    background: linear-gradient(135deg,var(--accent),var(--highlight));
    transform: scale(1.05);
    box-shadow: 0 6px 14px rgba(34,197,94,0.4);
  }
  .project h3{margin:0;font-size:16px; color:#fff; transition: color 0.3s ease;}
  .project h3:hover{color: var(--highlight);}
  .project p{margin:6px 0;color:var(--muted);font-size:14px}
  .project .links{display:flex;gap:8px;margin-top:8px}

  footer{
    margin-top:22px;
    color:var(--muted);
    font-size:13px;
    text-align:center;
    position: relative;
  }
  footer small{
    display:inline-block;
    position: relative;
    animation: sparkle 1.5s infinite;
  }
  @keyframes sparkle{
    0%{opacity:0;}
    50%{opacity:1;}
    100%{opacity:0;}
  }

  html{scroll-behavior:smooth;}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <img src="C:\Users\sknay\OneDrive\Pictures\WhatsApp Image 2025-08-14 at 18.08.30_3eaced69.jpg" alt="My Profile Picture" class="avatar" id="avatar">
        <div>
          <h1 id="prof-name">Shaik Nayeem</h1>
          <p class="lead" id="prof-title">AI & Data Science Student's Portfolio</p>
        </div>
      </div>
      <div class="actions">
        <button class="btn btn-primary" onclick="showSection('about')">About</button>
        <button class="btn btn-primary" onclick="showSection('projects')">Projects</button>
        <button class="btn btn-primary" onclick="showSection('contact')">Contact</button>
        <button class="btn btn-primary" onclick="showSection('quicklinks')">Quick Links</button>
      </div>
    </header>

    <!-- About -->
    <div id="about" class="tab-section">
      <div class="card">
        <h3>About</h3>
        <p id="about-text">Hi THIS is <strong>Shaik Nayeem</strong>. I build machine learning models and develop user-friendly web demos to showcase their practical applications. I am an active learner with a passion for exploring new technologies, and a critical thinker who enjoys solving problems with innovative and efficient solutions.</p>
        <hr />
        <dl class="meta">
          <dt>Email</dt><dd id="email">sknayeemnayeem916@gmail.com</dd>
          <dt>Location</dt><dd id="location">Vijayawada, India</dd>
          <dt>Skills</dt><dd id="skills">Python, Java, Flask, SQL, PHP, MongoDB, Git</dd>
        </dl>
      </div>
    </div>

    <!-- Projects -->
    <div id="projects" class="tab-section">
      <div class="card">
        <h3>Projects</h3>
        <div class="projects">
          <div class="project">
            <div class="thumb">PC</div>
            <div>
              <h3>Diabetes Prediction</h3>
              <p class="muted">SVM classifies data by finding the best separating hyperplane, while Random Forest combines multiple decision trees for accurate diabetes prediction. A web application built with HTML and CSS allows users to enter patient details and view prediction results in a simple interface connected to the model.</p>
              <div class="links">
                <a class="btn" href="C:\Users\sknay\OneDrive\ドキュメント\ML project11.pptx" target="_blank">View PPT</a>
              </div>
            </div>
          </div>

          <div class="project">
            <div class="thumb">PP</div>
            <div>
              <h3>Pollen's Profiling Pollen Classifier</h3>
              <p class="muted">Developed a deep learning model using CNNs for automated classification of pollen grains from images. Integrated the model into a Flask-based web application with an HTML/CSS interface for user-friendly predictions.</p>
              <div class="links">
                <a class="btn" href="C:\Users\sknay\Downloads\Telegram Desktop\Pollen's Profiling final.docx" target="_blank">View DOCS</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Contact -->
    <div id="contact" class="tab-section">
      <div class="card">
        <h3>Contact</h3>
        <p class="muted">Looking for collaboration, internship, or project feedback? Reach out — I usually reply within a day.</p>
        <p><strong>Email:</strong> sknayeemnayeem916@gmail.com</p>
        <p><strong>Phone:</strong> 6300350551</p>
      </div>
    </div>

    <!-- Quick Links -->
    <div id="quicklinks" class="tab-section">
      <div class="card">
        <h3>Quick Links</h3>
        <p>
          <a href="https://github.com/Nayeem103110" target="_blank">GitHub</a> · 
          <a href="https://www.linkedin.com/in/shaik-nayeem-80a362285/" target="_blank">LinkedIn</a> · 
          <a href="D:\Shaik Nayeem.pdf" target="_blank">Resume (PDF)</a>
        </p>
      </div>
    </div>

    <footer>
      <small>Crafted with passion and precision. Connect with me on GitHub & LinkedIn.</small>
    </footer>
  </div>

  <script>
    // By default, hide all sections (only profile is visible)
    document.addEventListener("DOMContentLoaded", () => {
      const sections = document.querySelectorAll('.tab-section');
      sections.forEach(sec => sec.style.display = 'none');
    });

    // Function to show selected tab and hide others
    function showSection(sectionId) {
      const sections = document.querySelectorAll('.tab-section');
      sections.forEach(sec => sec.style.display = 'none'); 
      document.getElementById(sectionId).style.display = 'block';
    }
  </script>
</body>
</html>
