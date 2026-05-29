---
layout: default
title: Services
---

<div class="hero">
  <h1>Commercial Concrete Solutions</h1>
  <p>Professional Services for Commercial Projects</p>
</div>

At Erazo Concrete LLC, we specialize in commercial-grade concrete work with professional craftsmanship and engineering expertise.

<div class="services-grid">
  {% for service in site.services %}
    <div class="service-card">
      <h3>{{ service.title }}</h3>
      <p>{{ service.content | strip_html | truncatewords: 20 }}</p>
      <a href="{{ service.url }}" class="btn">Learn More</a>
    </div>
  {% endfor %}
</div>

## Why Choose Erazo Concrete?

- **Engineering Expertise** - Engineered solutions meeting all building codes
- **Professional Team** - Commercial concrete specialists
- **Quality Materials** - Premium concrete and finishes
- **Competitive Pricing** - Fair prices for commercial projects
- **Reliable Delivery** - On-time project completion
- **1-Year Warranty** - All work backed by comprehensive warranty
- **Free Consultation** - Professional assessment at no cost

## Ready to Get Started?

[Request a Free Quote](/contact/){: .btn}
