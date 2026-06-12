---
layout: default
title: Home
---

<style>
  /* Removes misaligned borders and shadows to make the boxes sit perfectly flush */
  .hero, .hero-content, .service-card {
    border: none !important;
    box-shadow: none !important;
    outline: none !important;
  }
</style>

<div class="hero">
  <div class="hero-content">
    <h1>Concrete Solutions</h1>
    <p>Commercial concrete solutions focused on quality, durability, and on-time project execution.</p>
    <div class="hero-actions">
      <a href="/contact/" class="btn">Get Your Quote Now</a>
      <a href="#services" class="btn btn-secondary">View Services</a>
    </div>
  </div>
</div>

<section class="services-section" id="services">
  <div class="section-header">
    <h2>Our Services</h2>
    <p class="section-subtitle">Foundations, Footings, Slabs, Piers, Grade Beams, etc.</p>
  </div>
  
  <div class="services-grid">
    <div class="service-card" id="commercial-installation">
      <div class="image-gallery">
        {% for file in site.static_files %}
          {% if file.path contains '/assets/images/foundations/' %}
            <img src="{{ file.path | relative_url }}" alt="Commercial foundation project">
          {% endif %}
        {% endfor %}
        {% for file in site.static_files %}
          {% if file.path contains '/assets/images/industrial/' %}
            <img src="{{ file.path | relative_url }}" alt="Industrial project">
          {% endif %}
        {% endfor %}
      </div>
      <div class="service-content">
        <h3>Commercial Installation</h3>
        <p>Building foundations, slabs, and industrial structures engineered for performance and compliance.</p>
        <a href="/services/foundation/" class="service-link">Learn more →</a>
      </div>
    </div>

    <div class="service-card" id="residential-projects">
      <div class="image-gallery">
        {% for file in site.static_files %}
          {% if file.path contains '/assets/images/residential/' %}
            <img src="{{ file.path | relative_url }}" alt="Residential project">
          {% endif %}
        {% endfor %}
      </div>
      <div class="service-content">
        <h3>Residential Projects</h3>
        <p>Patios, walkways, and exterior surfaces designed for durability and aesthetic appeal.</p>
        <a href="/services/driveways/" class="service-link">Learn more →</a>
      </div>
    </div>
  </div>
</section>

<section style="background: linear-gradient(to bottom, transparent, var(--light-bg) 25%, var(--light-bg) 75%, transparent); padding: 120px 20px; text-align: center; margin: 60px 0;">
  <div style="max-width: 600px; margin: 0 auto;">
    <h2 style="font-family: Georgia, serif; font-style: italic; margin-top: 0;">Start Your Project</h2>
    <p style="margin-bottom: 30px; line-height: 1.6;">Get your quote now and project assessment from our team.</p>
    <a href="/contact/" class="btn">Get Your Quote Now</a>
  </div>
</section>
