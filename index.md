---
layout: default
title: Home
---

<<<<<<< HEAD
<div style="float: right; margin-left: 20px; margin-bottom: 20px; z-index: 10; position: relative;">
  <img src="/assets/LOGOTIPO%20Sien%20FONDO.jpeg" alt="Erazo Concrete Logo" style="max-height: 150px;" />
</div>

<div class="hero">
  <h1>Commercial Foundation Specialists</h1>
  <p>Expert Concrete Foundations for Commercial Construction</p>
  <p style="margin-top: 20px;"><a href="/contact/" class="btn" style="display: inline-block;">Get Your Free Quote</a></p>
</div>

=======
<div class="hero">
  <h1>Commercial Foundation Specialists</h1>
  <p>Expert Concrete Foundations for Commercial Construction</p>
  <p style="margin-top: 20px;"><a href="/contact/" class="btn" style="display: inline-block;">Get Your Free Quote</a></p>
</div>

>>>>>>> a4e515df28d6c52cac91c7461c5e6c17d7878f1f
## Welcome to Erazo Concrete LLC

Your trusted partner for professional commercial concrete foundations. We specialize in engineered concrete solutions that meet the highest standards.

## Our Services

<div class="services-grid">
  <div class="service-card">
    <div class="service-icon">🏗️</div>
    <h3>New Foundations</h3>
    <p>Engineered concrete foundations for commercial buildings and construction projects.</p>
    <a href="/services/foundation/" class="btn btn-secondary">Learn More</a>
  </div>
  <div class="service-card">
    <div class="service-icon">🏭</div>
    <h3>Industrial Concrete</h3>
    <p>Heavy-duty concrete solutions for industrial and commercial applications.</p>
    <a href="/services/foundation/" class="btn btn-secondary">Learn More</a>
  </div>
  <div class="service-card">
    <div class="service-icon">🛠️</div>
    <h3>Concrete Driveways</h3>
    <p>Commercial-grade driveways for loading areas and access routes.</p>
    <a href="/services/driveways/" class="btn btn-secondary">Learn More</a>
  </div>
  <div class="service-card">
    <div class="service-icon">✅</div>
    <h3>1-Year Warranty</h3>
    <p>All work backed by comprehensive warranty for peace of mind.</p>
  </div>
</div>

## Our Process

<div style="background: #f8f9fa; padding: 30px; border-radius: 8px; margin: 40px 0;">
  <h3 style="text-align: center; margin-top: 0;">Foundation Work Steps</h3>
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; margin-top: 30px;">
    <div style="text-align: center;">
      <div style="font-size: 2.5em; margin-bottom: 10px;">📋</div>
      <strong>1. Site Assessment</strong>
      <p>Evaluate soil conditions and design requirements</p>
    </div>
    <div style="text-align: center;">
      <div style="font-size: 2.5em; margin-bottom: 10px;">🔍</div>
      <strong>2. Engineering Review</strong>
      <p>Review plans and structural specifications</p>
    </div>
    <div style="text-align: center;">
      <div style="font-size: 2.5em; margin-bottom: 10px;">🏗️</div>
      <strong>3. Excavation & Prep</strong>
      <p>Proper grading and base preparation</p>
    </div>
    <div style="text-align: center;">
      <div style="font-size: 2.5em; margin-bottom: 10px;">🚚</div>
      <strong>4. Concrete Pour</strong>
      <p>Professional application and finishing</p>
    </div>
    <div style="text-align: center;">
      <div style="font-size: 2.5em; margin-bottom: 10px;">⏱️</div>
      <strong>5. Curing & Testing</strong>
      <p>Proper curing and quality verification</p>
    </div>
    <div style="text-align: center;">
      <div style="font-size: 2.5em; margin-bottom: 10px;">📜</div>
      <strong>6. Documentation</strong>
      <p>All certifications and compliance records</p>
    </div>
  </div>
</div>

## ⭐ 1-Year Warranty Guarantee

All our foundation work is backed by a **comprehensive 1-year warranty**. We guarantee structural integrity, proper installation, and full compliance with building codes. Your investment is protected.

## Recent Projects

<div class="projects-grid">
  {% for project in site.projects %}
    <div class="project-card">
      <div class="project-image">
        {% if project.image %}
          <img src="{{ project.image }}" alt="{{ project.title }}">
        {% else %}
          📸
        {% endif %}
      </div>
      <div class="project-content">
        <span class="project-category">{{ project.category }}</span>
        <h3 class="project-title">{{ project.title }}</h3>
        <p>{{ project.description | truncatewords: 20 }}</p>
        <a href="{{ project.url }}" class="btn btn-secondary">View Details</a>
      </div>
    </div>
  {% endfor %}
</div>

## What Our Clients Say

> "Erazo Concrete delivered professional work that met all our engineering requirements. Great to work with and thorough communication throughout."  
> — *ABC Development Corp., Commercial Client*

> "Best concrete contractor we've worked with. Professional, reliable, and on time."  
> — *Construction Manager*

## Ready to Get Started?

Start your commercial project with proven foundation expertise.

<<<<<<< HEAD
[Request Your Free Quote](/contact/){: .btn}
=======
[Request Your Free Quote](/contact/){: .btn}
>>>>>>> a4e515df28d6c52cac91c7461c5e6c17d7878f1f
