---
layout: default
title: Services
---

<section class="page-hero">
  <div class="page-hero-content">
    <h1>Services</h1>
    <p>Concrete services for commercial and industrial projects with clear planning and steady coordination.</p>
  </div>
</section>

<section class="content-panel">
  <p>Erazo Concrete provides commercial concrete services with a focus on staying on track and keeping clients informed at every stage.</p>
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
    <p>From site evaluation through finishing, we provide clear communication, progress updates, and dependable execution on every concrete job.</p>
  </div>
</section>

<section class="quote-panel">
  <div class="quote-panel-content">
    <h2>Ready to review your project?</h2>
    <p>Contact us for a free commercial quote and quick project assessment.</p>
    <a href="/contact/" class="btn">Request a Quote</a>
  </div>
</section>
