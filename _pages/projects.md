---
layout: page
title: Projects
permalink: /projects/
description: A collection of my work and side projects
nav: false
---

{% include back_button.html %}

<style>
  .bento-card {
    background-color: var(--global-card-bg-color); /* Adapts to theme */
    border: 1px solid var(--global-divider-color);
    border-radius: 15px;
    padding: 25px;
    height: 100%;
    transition: transform 0.2s, border-color 0.2s, box-shadow 0.2s;
  }
  /* Dark mode specific override if you want them properly dark */
  body.dark .bento-card {
    background-color: #1e1e1e;
    border-color: #333;
  }
  
  .bento-card:hover {
    transform: translateY(-5px);
    border-color: var(--global-theme-color);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  }
  
  .project-icon {
    font-size: 3rem;
    margin-bottom: 15px;
    color: var(--global-theme-color); /* Uses your site's main color */
  }
  
  .tech-pill {
    background-color: var(--global-hover-color);
    border: 1px solid var(--global-divider-color);
    color: var(--global-text-color);
    font-size: 0.75rem;
    padding: 4px 10px;
    border-radius: 12px;
    margin-right: 5px;
    margin-bottom: 5px;
    display: inline-block;
  }
</style>

<div class="row">
  
  <div class="col-md-4 mb-4">
    <div class="bento-card">
      <div class="project-icon">
        <i class="fas fa-car-side"></i> 
      </div>
      <h4>Autonomous Donkey Car</h4>
      <p class="text-muted">
        Built an autonomous car using a Raspberry Pi 5 and OAK-D-Lite camera. Implemented path following and computer vision for lane detection.
      </p>
      <div class="mt-3">
        <span class="tech-pill">Python</span>
        <span class="tech-pill">OpenCV</span>
        <span class="tech-pill">Raspberry Pi</span>
        <span class="tech-pill">DonkeyCar</span>
      </div>
    </div>
  </div>

  <div class="col-md-4 mb-4">
    <div class="bento-card">
      <div class="project-icon">
        <i class="fas fa-palette"></i>
      </div>
      <h4>GAN Image Colorizer</h4>
      <p class="text-muted">
        Created a U-Net GAN model with PyTorch to colorize black and white images. Trained on custom datasets to learn realistic color mapping.
      </p>
      <div class="mt-3">
        <span class="tech-pill">PyTorch</span>
        <span class="tech-pill">GANs</span>
        <span class="tech-pill">Python</span>
      </div>
    </div>
  </div>

  <div class="col-md-4 mb-4">
    <div class="bento-card">
      <div class="project-icon">
        <i class="fas fa-book-open"></i>
      </div>
      <h4>Shakespeare LSTM</h4>
      <p class="text-muted">
        Trained a Long Short-Term Memory (LSTM) network on 40k lines of Shakespeare to generate text in the Bard's style.
      </p>
      <div class="mt-3">
        <span class="tech-pill">TensorFlow</span>
        <span class="tech-pill">NLP</span>
        <span class="tech-pill">Deep Learning</span>
      </div>
    </div>
  </div>

</div>