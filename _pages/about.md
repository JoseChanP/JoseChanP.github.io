---
layout: about
title: home
permalink: /
subtitle: # Keep this empty
---

<div class="hero-section text-center">
  
  <img src="{{ '/assets/img/prof_pic.jpg' | relative_url }}" 
       alt="Jose A. Chan Pineda" 
       class="hero-image rounded-circle">

  <h1 class="hero-name">Jose A. Chan Pineda</h1>
  <h2 class="hero-subtitle">CS & Statistics @ UCSD | ML & Robotics Researcher</h2>

  <p class="hero-intro">
    I am a double major in Computer Science and Probability & Statistics, passionate about bridging the gap between software and the physical world. My work focuses on <strong>Machine Learning</strong>, <strong>Computer Vision</strong>, and <strong>Embodied AI</strong>—building autonomous systems that can perceive, plan, and act in real-time.
  </p>

  <div class="container my-5">
    <div class="row justify-content-center">
      
      <div class="col-md-5 mb-3">
        <a href="{{ '/projects/' | relative_url }}" class="text-decoration-none">
          <div class="p-4 rounded-3 text-center hero-nav-card">
            <i class="fas fa-code fa-2x mb-3" style="color: var(--global-theme-color)"></i>
            <h4 class="m-0">Projects</h4>
            <p class="small text-muted m-0">View my technical work</p>
          </div>
        </a>
      </div>

      <div class="col-md-5 mb-3">
        <a href="{{ '/education/' | relative_url }}" class="text-decoration-none">
          <div class="p-4 rounded-3 text-center hero-nav-card">
            <i class="fas fa-graduation-cap fa-2x mb-3" style="color: var(--global-theme-color)"></i>
            <h4 class="m-0">Education</h4>
            <p class="small text-muted m-0">Degrees & Certifications</p>
          </div>
        </a>
      </div>

    </div>
  </div>

  <div class="hero-social">
    <a href="https://github.com/JoseChanP" target="_blank" class="mx-2 text-decoration-none">
      <i class="fab fa-github fa-2x"></i>
    </a>
    <a href="https://linkedin.com/in/jose-chan-89909925b" target="_blank" class="mx-2 text-decoration-none">
      <i class="fab fa-linkedin fa-2x"></i>
    </a>
    <a href="mailto:Jcp316anton@gmail.com" class="mx-2 text-decoration-none">
      <i class="fas fa-envelope fa-2x"></i>
    </a>
  </div>

</div>

<style>
  .hero-section { padding: 60px 0 40px; }
  .hero-image {
    width: 180px; height: 180px; object-fit: cover;
    border: 5px solid var(--global-bg-color);
    box-shadow: 0 10px 25px rgba(0,0,0,0.1);
    margin-bottom: 25px;
  }
  .hero-name { font-weight: 800; font-size: 3.5rem; margin-bottom: 10px; }
  .hero-subtitle {
    font-weight: 400; font-size: 1.5rem;
    color: var(--global-text-color-light);
    margin-bottom: 25px;
  }
  .hero-intro {
    max-width: 700px; margin: 0 auto 35px auto;
    font-size: 1.15rem; line-height: 1.6;
  }
  .hero-social a { color: var(--global-text-color-light); transition: color 0.3s ease; }
  .hero-social a:hover { color: var(--global-theme-color); }

  /* Navigation Card Styles */
  .hero-nav-card {
    background-color: var(--global-bg-color); /* Adapts to light/dark mode */
    border: 1px solid var(--global-divider-color);
    transition: all 0.2s ease-in-out;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .hero-nav-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
    border-color: var(--global-theme-color);
  }
  .hero-nav-card h4 { color: var(--global-text-color); }
</style>