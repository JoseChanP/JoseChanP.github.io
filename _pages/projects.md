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
  /* 1. The "Beefy" Card Style */
  .bento-card {
    background-color: #121212; /* Deep dark background */
    border: 1px solid #333;
    border-radius: 16px;
    overflow: hidden;
    height: 100%;       /* Fills the column height */
    min-height: 550px;  /* FORCES the card to be tall/big */
    display: flex;
    flex-direction: column;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  /* Dark mode check */
  body.dark .bento-card {
    background-color: #1e1e1e;
    border-color: #333;
  }

  .bento-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 15px 35px rgba(0,0,0,0.5);
    border-color: #666;
  }

  /* 2. Taller Header Image */
  .project-header-img {
    width: 100%;
    height: 220px; /* Increased from 180px to make it pop */
    object-fit: cover;
    border-bottom: 1px solid #222;
  }

  /* 3. Spacious Content Area */
  .card-content {
    padding: 30px; /* Increased padding for that "big card" feel */
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  /* 4. Typography Updates */
  .bento-card h4 {
    color: #fff;
    font-weight: 700;
    font-size: 1.4rem;
    margin-bottom: 15px;
  }
  
  .bento-card p {
    color: #bbb;
    font-size: 0.95rem;
    line-height: 1.6; /* More spacing between lines */
    margin-bottom: 25px;
  }

  /* 5. Tech Pills */
  .tech-stack {
    margin-bottom: 25px;
  }
  
  .tech-pill {
    background-color: #222;
    border: 1px solid #333;
    color: #e0e0e0;
    font-size: 0.75rem;
    font-weight: 500;
    padding: 6px 12px;
    border-radius: 20px;
    margin-right: 6px;
    margin-bottom: 6px;
    display: inline-block;
  }

  /* 6. Bottom Button */
  .btn-code {
    background-color: transparent;
    border: 1px solid #444;
    color: #fff;
    padding: 10px 20px;
    border-radius: 8px;
    font-size: 0.9rem;
    font-weight: 600;
    display: inline-flex;
    align-items: center;
    transition: all 0.2s;
    width: fit-content;
    text-decoration: none !important;
    margin-top: auto; /* Pushes button to the very bottom */
  }

  .btn-code:hover {
    background-color: #333;
    border-color: #777;
    color: #fff;
  }
</style>

<div class="row">
  
  <div class="col-md-4 mb-5">
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
          <span class="tech-pill">OAK-D (CV)</span>
          <span class="tech-pill">Docker</span>
          <span class="tech-pill">Raspberry Pi 5</span>
          <span class="tech-pill">Python</span>
        </div>

        <a href="https://github.com/UCSD-ECEMAE-148/fall-2025-final-project-team-10" target="_blank" class="btn-code">
          <i class="fab fa-github mr-2"></i> View Code
        </a>
      </div>
    </div>
  </div>

  <div class="col-md-4 mb-5">
    <div class="bento-card">
      <img src="{{ '/assets/img/odom.gif' | relative_url }}" class="project-header-img" alt="Odometry">
      
      <div class="card-content">
        <h4>Diff-Drive Odometry</h4>
        <p>
          Developed a custom kinematic model for a differential drive robot to track pose $(x, y, \theta)$ solely from wheel encoder data. Analyzed error propagation and optimized trajectory tracking accuracy by implementing a Runge-Kutta integration method to reduce drift over long paths.
        </p>
        
        <div class="tech-stack">
          <span class="tech-pill">Python</span>
          <span class="tech-pill">NumPy</span>
          <span class="tech-pill">Matplotlib</span>
          <span class="tech-pill">Kinematics</span>
          <span class="tech-pill">Control Theory</span>
        </div>

        <a href="https://github.com/JoseChanP/your-odom-repo" target="_blank" class="btn-code">
          <i class="fab fa-github mr-2"></i> View Code
        </a>
      </div>
    </div>
  </div>

  <div class="col-md-4 mb-5">
    <div class="bento-card">
      <img src="{{ '/assets/img/recommender.png' | relative_url }}" class="project-header-img" alt="Recommender System">
      
      <div class="card-content">
        <h4>Personalized Recommender</h4>
        <p>
          Built a rating prediction engine using latent factor models and collaborative filtering. Implemented <strong>Jaccard</strong> and <strong>Pearson</strong> similarity metrics to analyze user behavior. The final model utilizes matrix factorization to predict user preferences for unrated items with high accuracy (low MSE).
        </p>
        
        <div class="tech-stack">
          <span class="tech-pill">TensorFlow</span>
          <span class="tech-pill">Pandas</span>
          <span class="tech-pill">Scikit-Learn</span>
          <span class="tech-pill">Matplotlib</span>
          <span class="tech-pill">Data Science</span>
        </div>

        <a href="https://github.com/JoseChanP/your-recommender-repo" target="_blank" class="btn-code">
          <i class="fab fa-github mr-2"></i> View Code
        </a>
      </div>
    </div>
  </div>

</div>