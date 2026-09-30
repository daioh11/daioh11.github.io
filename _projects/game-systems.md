---
layout: project
title: "Game Systems"
---

<p class="project-intro">
  Collection of general gameplay mechanics, core architecture, and supporting utility frameworks.
</p>

<!-- Здесь будут располагаться блоки с демками систем (demo-grid) -->

<!-- Пример заготовки под будущую систему (раскомментируй и заполни при необходимости):

<div class="demo-grid">
  <div class="video-container">
    <iframe 
      src="https://www.youtube.com/embed/ТВОЙ_ID_ВИДЕО" 
      title="System Name Demo" 
      frameborder="0" 
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
      allowfullscreen>
    </iframe>
  </div>

  <div class="demo-info">
    <h3>System Name</h3>
    <p>
      System short description and purpose overview.
    </p>

    <ul class="feature-list">
      <li><strong>Feature 1:</strong> Specification and details.</li>
      <li><strong>Feature 2:</strong> Specification and details.</li>
    </ul>
  </div>
</div>
-->

<!-- Стили, полностью единые с остальными страницами проектов -->
<style>
  .project-intro {
    font-size: 1.1em;
    color: #e6e6fa;
    margin-bottom: 30px;
    border-left: 3px solid #ff005d;
    padding-left: 15px;
  }

  .demo-grid {
    display: grid;
    grid-template-columns: 1.2fr 1fr;
    gap: 25px;
    align-items: start;
    margin-bottom: 40px;
    background: rgba(16, 15, 21, 0.6);
    border: 1px solid #2a2c3d;
    padding: 20px;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.5);
  }

  .video-container {
    position: relative;
    width: 100%;
    padding-bottom: 56.25%;
    height: 0;
    border: 1px solid #ff005d;
    box-shadow: 0 0 12px rgba(255, 0, 93, 0.35);
    background-color: #000;
  }

  .video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

  .demo-info h3 {
    margin-top: 0;
    color: #00f3ff;
    font-size: 1.3em;
    text-shadow: 0 0 5px rgba(0, 243, 255, 0.4);
    border-bottom: 1px solid #2a2c3d;
    padding-bottom: 8px;
  }

  .demo-info p {
    color: #e6e6fa;
    font-size: 0.95em;
    line-height: 1.5;
  }

  .feature-list {
    list-style-type: none;
    padding-left: 0;
    margin-top: 15px;
  }

  .feature-list li {
    position: relative;
    padding-left: 18px;
    margin-bottom: 10px;
    font-size: 0.9em;
    color: #d1d2e0;
  }

  .feature-list li::before {
    content: '>';
    position: absolute;
    left: 0;
    color: #ff005d;
    font-weight: bold;
  }

  .feature-list strong {
    color: #ffffff;
  }

  @media (max-width: 768px) {
    .demo-grid {
      grid-template-columns: 1fr;
    }
  }
</style>