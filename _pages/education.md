---
layout: page
title: Education
permalink: /education/
description: Academic background and qualifications
nav: true
nav_order: 3
---

{% include back_button.html %}

<style>
    header.post-header {
    display: none !important;
  }
  
  /* 1. Force Wide Layout */
  .container, .container-fluid {
    max-width: 1600px !important;
    padding-left: 30px;
    padding-right: 30px;
  }

  /* 2. Big Title Styling */
  .page-title {
    font-size: 4rem !important;
    font-weight: 800;
    margin-bottom: 1rem;
    letter-spacing: -1px;
  }
  
  .title-icon {
    color: var(--global-theme-color);
    margin-right: 15px;
    opacity: 0.8;
  }

  /* 3. The "Beefy" Education Card */
  .edu-card {
    background-color: #121212;
    border: 1px solid #333;
    border-radius: 20px;
    padding: 40px; /* Massive padding */
    margin-bottom: 30px;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  body.dark .edu-card {
    background-color: #1a1a1a;
    border-color: #333;
  }

  .edu-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 20px 40px rgba(0,0,0,0.4);
    border-color: #666;
  }

  /* 4. Typography Scaling */
  .edu-institution {
    font-size: 2rem; /* Big University Name */
    font-weight: 700;
    color: #fff;
    margin-bottom: 5px;
  }

  .edu-degree {
    font-size: 1.5rem; /* Big Degree Name */
    color: #ddd;
    margin-bottom: 15px;
    font-weight: 500;
  }

  .edu-meta {
    font-size: 1.1rem;
    color: #aaa;
    line-height: 1.6;
  }

  /* 5. Badges & Pills */
  .custom-badge {
    font-size: 0.9rem;
    padding: 6px 12px;
    border-radius: 8px;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }

  .badge-grad { background-color: #0d6efd; color: white; }
  .badge-undergrad { background-color: #6c757d; color: white; }
  .badge-cert { background-color: #198754; color: white; }

</style>

<div class="mb-5 mt-4">
  <h1 class="page-title">
    <span class="title-icon"><i class="fas fa-graduation-cap"></i></span>Education
  </h1>
  <p class="text-muted" style="font-size: 1.2rem;">My academic journey and professional certifications.</p>
</div>

<div class="row">
  
  <div class="col-12">
    <div class="edu-card">
      <div class="row align-items-center">
        <div class="col-md-1 d-none d-md-block text-center">
          <i class="fas fa-user-graduate fa-4x" style="color: #ffd700;"></i>
        </div>
        
        <div class="col-md-11">
          <div class="d-flex justify-content-between align-items-start">
            <div>
              <div class="edu-institution">University of California, San Diego</div>
              <div class="edu-degree">M.S. in Computer Science</div>
            </div>
            <span class="custom-badge badge-grad">Expected 2027</span>
          </div>
          
          <div class="edu-meta mt-3">
            <p class="mb-2">
              <span class="text-white border border-secondary rounded px-2 py-1 mr-2" style="font-size: 0.9em;">BS/MS Program</span>
              Specialization in <strong>Artificial Intelligence & Machine Learning</strong>
            </p>
            <p class="mb-0 text-muted"><em>Starting graduate coursework in January 2026.</em></p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="col-12">
    <div class="edu-card">
      <div class="row align-items-center">
        <div class="col-md-1 d-none d-md-block text-center">
          <i class="fas fa-university fa-4x text-muted"></i>
        </div>
        
        <div class="col-md-11">
          <div class="d-flex justify-content-between align-items-start">
            <div>
              <div class="edu-institution">University of California, San Diego</div>
              <div class="edu-degree">Double Major B.S.</div>
            </div>
            <span class="custom-badge badge-undergrad">Expected 2026</span>
          </div>
          
          <div class="mt-3">
            <div class="d-flex align-items-center mb-2">
              <i class="fas fa-check-circle text-success mr-3" style="font-size: 1.2rem;"></i>
              <span style="font-size: 1.3rem; color: #ccc;">Computer Science</span>
            </div>
            <div class="d-flex align-items-center mb-3">
              <i class="fas fa-check-circle text-success mr-3" style="font-size: 1.2rem;"></i>
              <span style="font-size: 1.3rem; color: #ccc;">Probability & Statistics</span>
            </div>
          </div>

          <div class="edu-meta border-top border-secondary pt-3 mt-3">
            <div class="row">
              <div class="col-md-3">
                <strong>GPA:</strong> <span class="text-white">3.935 / 4.0</span>
              </div>
              <div class="col-md-9">
                <strong>Honors:</strong> Provost Honors, Earl Warren College
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="col-12 mt-4">
    <h2 class="mb-4" style="font-weight: 700; color: #ddd;">Certifications</h2>
    <div class="edu-card py-4"> <div class="row align-items-center">
        <div class="col-md-1 d-none d-md-block text-center">
          <i class="fas fa-robot fa-3x" style="color: #666;"></i>
        </div>
        <div class="col-md-11">
           <div class="d-flex justify-content-between align-items-center">
             <h3 class="mb-0 text-white" style="font-size: 1.5rem;">ROS2 & Robotics Developer</h3>
             <span class="custom-badge badge-cert">Issued 2024</span>
           </div>
           <p class="text-muted mt-2 mb-0" style="font-size: 1.1rem;">
             <strong>The Construct Sim:</strong> Comprehensive training in Linux for Robotics, Python 3, and ROS 2 (Foxy/Humble) Navigation & Manipulation stacks.
           </p>
        </div>
      </div>
    </div>
  </div>

</div>