---
layout: page
title: Projects
permalink: /projects/
description: A collection of my work and side projects
nav: true
---

{% include back_button.html %}

<style>
  /* 1. Card Container - Matches the reference dark style */
  .bento-card {
    background-color: #121212; /* Deep dark background */
    border: 1px solid #333;
    border-radius: 16px;
    overflow: hidden;
    height: 100%;
    display: flex;
    flex-direction: column;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  .bento-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 10px 30px rgba(0,0,0,0.5);
    border-color: #555;
  }

  /* 2. Header Image/GIF */
  .project-header-img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-bottom: 1px solid #222;
  }

  /* 3. Content Padding */
  .card-content {
    padding: 24px;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  /* 4. Typography */
  .bento-card h4 {
    color: #fff;
    font-weight: 700;
    margin-bottom: 10px;
  }
  
  .bento-card p {
    color: #bbb; /* Softer grey text */
    font-size: 0.95rem;
    line-height: 1.5;
    margin-bottom: 20px;
  }

  /* 5. Tech Pills (The small bubbles) */
  .tech-stack {
    margin-bottom: 20px;
  }
  
  .tech-pill {
    background-color: #222;
    border: 1px solid #333;
    color: #e0e0e0;
    font-size: 0.75rem;
    font-weight: 500;
    padding: 4px 12px;
    border-radius: 20px; /* Fully rounded caps */
    margin-right: 6px;
    margin-bottom: 6px;
    display: inline-block;
  }

  /* 6. The 'Code' Button */
  .btn-code {
    background-color: transparent;
    border: 1px solid #444;
    color: #fff;
    padding: 8px 16px;
    border-radius: 8px;
    font-size: 0.85rem;
    font-weight: 600;
    display: inline-flex;
    align-items: center;
    transition: all 0.2s;
    width: fit-content;
    text-decoration: none !important; /* Force remove underline */
  }

  .btn-code:hover {
    background-color: #333;
    border-color: #666;
    color: #fff;
  }
</style>

<div class="row">
  
  <div class="col-md-4 mb-4">
    <div class="bento-card">
      <img src="{{ '/assets/img/lost_found.gif' | relative_url }}" class="project-header-img" alt="Lost Found Bot">
      
      <div class="card-content">
        <h4>Lost & Found Robot</h4>
        <p>
          An autonomous mobile robot designed to map unknown environments and retrieve objects using Frontier Exploration and Visual Servoing.
        </p>
        
        <div class="tech-stack">
          <span class="tech-pill">ROS 2</span>
          <span class="tech-pill">Nav2</span>
          <span class="tech-pill">SLAM</span>
          <span class="tech-pill">OAK-D</span>
        </div>

        <a href="https://github.com/UCSD-ECEMAE-148/fall-2025-final-project-team-10" target="_blank" class="btn-code">
          <i class="fab fa-github mr-2"></i> Code
        </a>
      </div>
    </div>
  </div>

  <div class="col-md-4 mb-4">
    <div class="bento-card">
      <img src="{{ '/assets/img/odom.gif' | relative_url }}" class="project-header-img" alt="Odometry">
      
      <div class="card-content">
        <h4>Diff-Drive Odometry</h4>
        <p>
          Custom kinematic model for a differential drive robot to track pose (x, y, theta) from encoder data, optimized for trajectory accuracy.
        </p>
        
        <div class="tech-stack">
          <span class="tech-pill">Python</span>
          <span class="tech-pill">NumPy</span>
          <span class="tech-pill">Kinematics</span>
        </div>

        <a href="https://github.com/JoseChanP/your-odom-repo" target="_blank" class="btn-code">
          <i class="fab fa-github mr-2"></i> Code
        </a>
      </div>
    </div>
  </div>

  <div class="col-md-4 mb-4">
    <div class="bento-card">
      <img src="{{ '/assets/img/recommender.png' | relative_url }}" class="project-header-img" alt="Recommender System">
      
      <div class="card-content">
        <h4>Personalized Recommender</h4>
        <p>
          Rating prediction model using latent factor models and collaborative filtering (Jaccard/Pearson) to predict user preferences.
        </p>
        
        <div class="tech-stack">
          <span class="tech-pill">TensorFlow</span>
          <span class="tech-pill">Pandas</span>
          <span class="tech-pill">Scikit-Learn</span>
        </div>

        <a href="https://github.com/JoseChanP/your-recommender-repo" target="_blank" class="btn-code">
          <i class="fab fa-github mr-2"></i> Code
        </a>
      </div>
    </div>
  </div>

</div>