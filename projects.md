---
layout: default
title: Our Work
---

<style>
  /* Removes misaligned border from the hero box to sit flush */
  .hero {
    border: none !important;
    box-shadow: none !important;
  }
</style>

<div class="hero">
  <h1>Our Work</h1>
  <p>A showcase of our craftsmanship. As projects are completed, photos will be uploaded here to demonstrate our commitment to quality and client satisfaction.</p>
</div>

{% assign folder_names = "" %}
{% for file in site.static_files %}
  {% if file.path contains '/assets/images/projects/' %}
    {% assign parts = file.path | split: '/' %}
    {% if parts.size > 5 %}
      {% assign folder = parts[4] %}
      {% assign folder_with_delim = folder | append: "||" %}
      {% unless folder_names contains folder_with_delim %}
        {% assign folder_names = folder_names | append: folder_with_delim %}
      {% endunless %}
    {% endif %}
  {% endif %}
{% endfor %}
{% assign folders_array = folder_names | split: "||" %}

<div class="dynamic-projects-list" style="margin-top: 40px;">
  {% for folder in folders_array %}
    {% if folder != "" %}
      <div class="project-area" style="margin-bottom: 60px; padding: 30px; background: var(--light-bg); border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.05);">
        <h2 style="margin-top: 0; text-transform: capitalize; color: var(--text-color);">Current - {{ folder | replace: '-', ' ' | replace: '_', ' ' }}</h2>
        <div class="project-carousel" style="display: grid; gap: 15px; margin-top: 20px; min-height: 250px;">
          {% assign folder_path = '/assets/images/projects/' | append: folder | append: '/' %}
          {% for file in site.static_files %}
            {% if file.path contains folder_path %}
              <a href="{{ file.path | relative_url }}" target="_blank" rel="noopener noreferrer">
                <img src="{{ file.path | relative_url }}" alt="{{ folder }} project photo" style="width: 100%; height: 250px; object-fit: cover; border-radius: 8px;">
              </a>
            {% endif %}
          {% endfor %}
        </div>
      </div>
    {% endif %}
  {% endfor %}
</div>

## Ready to Start Your Project?

Let us bring your vision to life with reliable concrete work.

[Get Your Free Quote](/contact/){: .btn}