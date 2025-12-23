---
layout: about
title: home
permalink: /
subtitle: # Keep this empty
---

<div class="hero-section text-center">
  
  <img src="{{ '/assets/img/your-profile-pic.jpg' | relative_url }}" 
       alt="Jose A. Chan Pineda" 
       class="hero-image rounded-circle">

  <h1 class="hero-name">Jose A. Chan Pineda</h1>

  <h2 class="hero-subtitle">CS & Statistics @ UCSD | ML & Robotics Researcher</h2>

  <p class="hero-intro">
    I am a double major in Computer Science and Probability & Statistics, passionate about bridging the gap between software and the physical world. My work focuses on <strong>Machine Learning</strong>, <strong>Computer Vision</strong>, and <strong>Embodied AI</strong>—building autonomous systems that can perceive, plan, and act in real-time.
  </p>

  <div class="hero-buttons my-4">
    <a href="{{ '/projects/' | relative_url }}" class="btn btn-primary shadow-sm">View Projects</a>
    
    <a href="{{ '/assets/pdf/your-resume.pdf' | relative_url }}" target="_blank" class="btn btn-outline-primary shadow-sm">
      <i class="fas fa-download mr-1"></i> My Resume
    </a>
  </div>

  <div class="hero-social">
    <a href="https://github.com/JoseChanP" target="_blank" class="mx-2 text-decoration-none">
      <i class="fab fa-github fa-2x"></i>
    </a>
    <a href="https://linkedin.com/in/jose-chan-89909925b" target="_blank" class="mx-2 text-decoration-none">
      <i class="fab fa-linkedin fa-2x"></i>
    </a>
    <a href="Jcp316anton@gmail.com" class="mx-2 text-decoration-none">
      <i class="fas fa-envelope fa-2x"></i>
    </a>
  </div>

</div>

<div class="my-5"></div>

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
  .hero-buttons .btn {
    margin: 0 10px; padding: 12px 30px;
    border-radius: 50px; font-weight: 600;
    text-transform: uppercase; letter-spacing: 1px; font-size: 0.9rem;
  }
  .hero-social a { color: var(--global-text-color-light); transition: color 0.3s ease; }
  .hero-social a:hover { color: var(--global-theme-color); }
  body.dark .hero-image { box-shadow: 0 10px 25px rgba(255, 255, 255, 0.1); }
</style>