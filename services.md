---
layout: default
title: Services
---

<section class="page-hero">
  <div class="page-hero-content">
    <h1>Services</h1>
    <p>Concrete services for commercial and industrial projects that keep work moving.</p>
  </div>
</section>

<section class="content-panel">
  <p>Erazo Concrete provides commercial concrete services with a focus on keeping schedules on track and keeping clients informed through every phase.</p>
</section>

<div class="services-grid">
  {% for service in site.services %}
    <div class="service-card">
      <h3>{{ service.title }}</h3>
      <p>{{ service.content | strip_html | truncatewords: 20 }}</p>
      <a href="{{ service.url }}" class="btn">Learn More</a>
    </div>
  {% endfor %}
</div>

<section class="content-row">
  <div class="content-panel">
    <h2>Efficient Scheduling</h2>
    <ul>
      <li>Project timelines that stay on course</li>
      <li>Tasks coordinated for faster delivery</li>
      <li>Clear milestones and progress updates</li>
      <li>Responsive communication with every client</li>
    </ul>
  </div>
  <div class="content-panel">
    <h2>Our Process</h2>
    <p>We maintain project momentum from consultation through completion, with clear communication and reliable execution.</p>
  </div>
</section>

<section class="quote-panel">
  <div class="quote-panel-content">
    <h2>Ready to review your project?</h2>
    <p>Contact us for a free commercial quote and quick project assessment.</p>
    <a href="/contact/" class="btn">Request a Quote</a>
  </div>
</section>
