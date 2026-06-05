---
layout: default
title: Services
---

<section class="page-hero">
  <div class="page-hero-content">
    <h1>Commercial Concrete Services</h1>
    <p>Clear, professional service offerings for developers, contractors, and commercial construction teams.</p>
  </div>
</section>

<section class="content-panel">
  <p>Erazo Concrete focuses on commercial-grade concrete work with a disciplined approach to quality, cost, and schedule. Our service portfolio is built for buildings, industrial sites, and infrastructure projects.</p>
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
    <h2>Why Choose Erazo Concrete?</h2>
    <ul>
      <li>Engineering expertise aligned with commercial needs</li>
      <li>Premium materials and code-compliant installation</li>
      <li>Transparent pricing and dependable delivery</li>
      <li>Warranty-backed work for long-term confidence</li>
    </ul>
  </div>
  <div class="content-panel">
    <h2>Project Support</h2>
    <p>From site evaluation through finishing, we provide clear communication, progress updates, and professional execution on every concrete job.</p>
  </div>
</section>

<section class="quote-panel">
  <div class="quote-panel-content">
    <h2>Ready to review your project?</h2>
    <p>Contact us for a free commercial quote and quick project assessment.</p>
    <a href="/contact/" class="btn">Request a Quote</a>
  </div>
</section>
