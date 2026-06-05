---
layout: default
title: Services
---

<section class="page-hero">
  <div class="page-hero-content">
    <h1>Our Services</h1>
    <p>Professional concrete services for commercial and industrial projects.</p>
  </div>
</section>

<section class="content-panel">
  <p>Erazo Concrete provides commercial concrete services with a focus on quality, cost-effectiveness, and project delivery. We work on foundations, industrial installations, and commercial paving projects.</p>
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
    <h2>Why Choose Us</h2>
    <ul>
      <li>Professional concrete installation</li>
      <li>Code-compliant work and quality materials</li>
      <li>Transparent pricing</li>
      <li>Warranty protection on all work</li>
    </ul>
  </div>
  <div class="content-panel">
    <h2>Our Process</h2>
    <p>We provide professional service from initial consultation through project completion, with clear communication and reliable execution.</p>
  </div>
</section>

<section class="quote-panel">
  <div class="quote-panel-content">
    <h2>Ready to review your project?</h2>
    <p>Contact us for a free commercial quote and quick project assessment.</p>
    <a href="/contact/" class="btn">Request a Quote</a>
  </div>
</section>
