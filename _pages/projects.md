---
layout: page
title: Projects
permalink: /projects/
description: A collection of my work and side projects
nav: true
nav_order: 2
---

{% include back_button.html %}

<style>
  header.post-header {
    display: none !important;
  }
  
  /* 1. BREAK THE CONTAINER: Force the page to be wider */
  .container, .container-fluid {
    max-width: 1600px !important; /* Forces the layout to be much wider */
    padding-left: 30px;
    padding-right: 30px;
  }

  /* 2. The "Super Sized" Card */
  .bento-card {
    background-color: #121212;
    border: 1px solid #333;
    border-radius: 20px; /* More rounded */
    overflow: hidden;
    height: 100%;
    min-height: 600px; /* Massive height */
    display: flex;
    flex-direction: column;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  body.dark .bento-card {
    background-color: #1a1a1a;
    border-color: #333;
  }

  .bento-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 40px rgba(0,0,0,0.6);
    border-color: #777;
  }

  /* 3. Huge Header Image */
  .project-header-img {
    width: 100%;
    height: 260px; /* Very tall image area */
    object-fit: cover;
    border-bottom: 1px solid #222;
  }

  /* 4. Content Scaling */
  .card-content {
    padding: 35px; /* Massive padding */
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .bento-card h4 {
    color: #fff;
    font-weight: 800; /* Extra bold */
    font-size: 1.75rem; /* Huge Title */
    margin-bottom: 15px;
  }
  
  .bento-card p {
    color: #bbb;
    font-size: 1.05rem; /* Larger body text */
    line-height: 1.7;
    margin-bottom: 30px;
  }

  /* 5. Dense Tech Pills */
  .tech-stack {
    margin-bottom: 30px;
  }
  
  .tech-pill {
    background-color: #252525;
    border: 1px solid #333;
    color: #eee;
    font-size: 0.85rem; /* Bigger text in pills */
    font-weight: 500;
    padding: 8px 16px; /* Bigger bubbles */
    border-radius: 25px;
    margin-right: 8px;
    margin-bottom: 8px;
    display: inline-block;
  }

  /* 6. Big Title Styling */
  .page-title {
    font-size: 4rem !important; /* Massive "Projects" text */
    font-weight: 800;
    margin-bottom: 1rem;
    letter-spacing: -1px;
  }
  
  .title-icon {
    color: var(--global-theme-color);
    margin-right: 15px;
    opacity: 0.8;
  }
</style>

<div class="mb-5 mt-4">
  <h1 class="page-title">
    <span class="title-icon"><i class="fas fa-code"></i></span>Projects
  </h1>
  <p class="text-muted" style="font-size: 1.2rem;">A collection of my work in Robotics, Machine Learning, and Software Engineering.</p>
</div>

<div class="row">
  
  <div class="col-lg-4 col-md-6 mb-5">
    <div class="bento-card">
      <img src="{{ '/assets/img/lost_found.gif' | relative_url }}" class="project-header-img" alt="Lost Found Bot">
      
      <div class="card-content">
        <h4>Lost & Found Robot</h4>
        <p>
          An autonomous mobile robot designed to map unknown environments and retrieve objects. The system integrates <strong>Frontier Exploration</strong> and <strong>SLAM</strong> to map a room without human intervention. Once a target is identified, a custom <strong>Visual Servoing</strong> loop locks onto the object and navigates the robot for retrieval using a priority-based Twist Multiplexer.
        </p>
        
        <div class="tech-stack">
          <span class="tech-pill">ROS 2 (Foxy)</span>
          <span class="tech-pill">Nav2</span>
          <span class="tech-pill">SLAM Toolbox</span>
          <span class="tech-pill">OAK-D Camera</span>
          <span class="tech-pill">OpenCV</span>
          <span class="tech-pill">Visual Servoing</span>
          <span class="tech-pill">Twist Mux</span>
          <span class="tech-pill">Docker</span>
          <span class="tech-pill">Raspberry Pi 5</span>
          <span class="tech-pill">Python</span>
        </div>

        <a href="https://github.com/UCSD-ECEMAE-148/fall-2025-final-project-team-10" target="_blank" class="btn btn-outline-light mt-auto">
          <i class="fab fa-github mr-2"></i> View Code
        </a>
      </div>
    </div>
  </div>

  <div class="col-lg-4 col-md-6 mb-5">
    <div class="bento-card">
      <img src="{{ '/assets/img/odom.gif' | relative_url }}" class="project-header-img" alt="Odometry">
      

        
      <div class="card-content">
        <h4>Monocular Visual Odometry</h4>
        <p>
          Implemented a vision-based pose estimation pipeline using <strong>OpenCV</strong>. Utilized <strong>Lucas-Kanade Optical Flow</strong> to track features across frames and computed the <strong>Essential Matrix</strong> using RANSAC. Recovered the camera's rotation and translation $(R, t)$ to reconstruct the 3D trajectory and validated performance against ground truth sequences.
        </p>
        
        <div class="tech-stack">
          <span class="tech-pill">Python</span>
          <span class="tech-pill">OpenCV</span>
          <span class="tech-pill">NumPy</span>
          <span class="tech-pill">Optical Flow</span>
          <span class="tech-pill">Epipolar Geometry</span>
          <span class="tech-pill">Computer Vision</span>
        </div>

        <a href="https://github.com/JoseChanP/your-odom-repo" target="_blank" class="btn btn-outline-light mt-auto">
          <i class="fab fa-github mr-2"></i> View Code
        </a>
      </div>
    </div>
  </div>

  <div class="col-lg-4 col-md-6 mb-5">
    <div class="bento-card">
      <img src="{{ '/assets/img/recommender.png' | relative_url }}" class="project-header-img" alt="Recommender System">
      

        
      <div class="card-content">
        <h4>Transformer Recommender (SASRec)</h4>
        <p>
          Built a <strong>Self-Attentive Sequential Recommendation (SASRec)</strong> model using <strong>PyTorch</strong> and <strong>Transformer Encoders</strong>. The model processes user timelines with learned positional and genre embeddings to predict next-item interactions. Benchmarked performance against <strong>Markov Chains</strong> and Hybrid statistical baselines, achieving superior hit rates.
        </p>
        
        <div class="tech-stack">
          <span class="tech-pill">PyTorch</span>
          <span class="tech-pill">Transformers</span>
          <span class="tech-pill">Deep Learning</span>
          <span class="tech-pill">Pandas</span>
          <span class="tech-pill">Markov Chains</span>
          <span class="tech-pill">Sequential Modeling</span>
        </div>

        <a href="https://github.com/JoseChanP/Sequential-Recommender" target="_blank" class="btn btn-outline-light mt-auto">
          <i class="fab fa-github mr-2"></i> View Code
        </a>
      </div>
    </div>
  </div>

</div>