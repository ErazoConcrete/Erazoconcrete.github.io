---
layout: default
title: Our Projects
---

<div class="hero">
  <h1>Project Portfolio</h1>
  <p>Showcase of Our Professional Concrete Work</p>
</div>

Browse our portfolio of completed projects. Each project demonstrates our commitment to quality, attention to detail, and customer satisfaction.

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

## Ready to Start Your Project?

Let us bring your vision to life with professional concrete work.

[Get Your Free Quote](/contact/){: .btn}