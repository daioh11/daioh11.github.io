---
layout: project
title: "Combat Systems"
---

<p class="project-intro">
  Collection of modular systems and architecture designed for competitive fighting games.
</p>

<!-- Сетка для видео и описания -->
<div class="demo-grid">
  
  <!-- Левая колонка: Видео -->
  <div class="video-container">
    <iframe 
      src="https://www.youtube.com/embed/S3m8ek_ofow?si=tmhwxdQS6mY8D88s" 
      title="Hit System Demo" 
      frameborder="0" 
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
      allowfullscreen>
    </iframe>
  </div>

  <!-- Правая колонка: Описание и спецификации -->
  <div class="demo-info">
    <h3>Advanced Hit System</h3>
    <p>
      Deterministic hit detection and attack pipeline built for authoritative servers.
    </p>

    <ul class="feature-list">
      <li><strong>Server Validation:</strong> Full server-side security checks for attack state and execution.</li>
      <li><strong>Secured Attack Phases:</strong> Prevents desync, input manipulation, and illegal state transitions.</li>
      <li><strong>Attack Tokens:</strong> Unique token-based tracking to eliminate duplicate hit registration.</li>
      <li><strong>Lag Compensation:</strong> Precision-tuned client prediction and hitbox rollback registration.</li>
    </ul>
  </div>

</div>

<div class="demo-grid">
  <div class="video-container">
    <iframe 
      src="https://www.youtube.com/embed/S3m8ek_ofow?si=tmhwxdQS6mY8D88s" 
      title="Dash System Demo" 
      frameborder="0" 
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
      allowfullscreen>
    </iframe>
  </div>

  <div class="demo-info">
    <h3> Dash and Block System</h3>
    <p>
      Responsive mobility engine handling directional dashes, momentum preservation, and cancels.
    </p>

    <ul class="feature-list">
      <li><strong>Buffer & Inputs:</strong> Double-tap and macro buffering with configurable execution windows.</li>
      <li><strong>State Cancels:</strong> Instant attack-to-dash and dash-cancel mechanics for fluid combat flow.</li>
      <li><strong>I-Frames & Hurtboxes:</strong> Dynamic invincibility frame alignment synced across client/server.</li>
      <li><strong>Velocity Curve:</strong> Custom acceleration vectors with inertia retention on wave-dashes.</li>
    </ul>
  </div>
</div>

<!-- Стили конкретно для этой сетки -->
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
    grid-template-columns: 1.2fr 1fr; /* Левая колонка чуть шире правой */
    gap: 25px;
    align-items: start;
    margin-bottom: 40px;
    background: rgba(16, 15, 21, 0.6);
    border: 1px solid #2a2c3d;
    padding: 20px;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.5);
  }

  /* Контейнер видео для правильного пропорционального масштабирования (16:9) */
  .video-container {
    position: relative;
    width: 100%;
    padding-bottom: 56.25%; /* Соотношение сторон 16:9 */
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

  /* Адаптив для мобильных устройств (автоматически складывается в 1 колонку) */
  @media (max-width: 768px) {
    .demo-grid {
      grid-template-columns: 1fr;
    }
  }
</style>