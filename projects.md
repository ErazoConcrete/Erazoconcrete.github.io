---
layout: default
title: Our Work
---

<div class="hero">
  <h1>Our Work</h1>
  <p>Showcase of our pours and completed concrete projects</p>
</div>

Browse our portfolio of completed projects. Each project demonstrates our commitment to quality, attention to detail, and customer satisfaction.

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
        <h2 style="margin-top: 0; text-transform: capitalize; color: var(--text-color);">{{ folder | replace: '-', ' ' | replace: '_', ' ' }}</h2>
        <div class="image-gallery" style="max-width: 100%; margin-top: 20px; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 20px rgba(0,0,0,0.1);">
          {% assign folder_path = '/assets/images/projects/' | append: folder | append: '/' %}
          {% for file in site.static_files %}
            {% if file.path contains folder_path %}
              <img src="{{ file.path | relative_url }}" alt="{{ folder }} project photo" style="width: 100%; object-fit: cover; aspect-ratio: 16/9;">
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