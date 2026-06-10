---
layout: default
title: Residential Projects
category: driveway
---

<div class="hero">
  <h1>Residential Projects</h1>
  <p>Driveways, patios, and walkways poured with traditional care and honest labor.</p>
</div>

A good driveway or patio is the welcoming mat to your home. We've been pouring residential concrete with the kind of care that treats your yard like our own. No rushed jobs, just solid, honest flatwork meant to last for generations.

<div class="image-gallery">
  {% for file in site.static_files %}
    {% if file.path contains '/assets/images/driveways/' %}
      <img src="{{ file.path | relative_url }}" alt="Residential project">
    {% endif %}
  {% endfor %}
</div>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 30px; margin: 50px 0;">
  <div style="border: 2px solid var(--text-color); border-radius: 12px; padding: 25px; box-shadow: 6px 6px 0px var(--text-color); background: var(--light-bg);">
    <h3 style="margin-top: 0; font-family: Georgia, serif; font-style: italic;">Patios & Walkways</h3>
    <p>A place for family gatherings and quiet mornings. We shape and pour custom outdoor living spaces that become part of the home.</p>
  </div>
  <div style="border: 2px solid var(--text-color); border-radius: 12px; padding: 25px; box-shadow: 6px 6px 0px var(--text-color); background: var(--light-bg);">
    <h3 style="margin-top: 0; font-family: Georgia, serif; font-style: italic;">Built to Weather</h3>
    <p>We use premium mixes that stand up to the freezing winters and hot summers. No cutting corners on the sub-base or the finish.</p>
  </div>
  <div style="border: 2px solid var(--text-color); border-radius: 12px; padding: 25px; box-shadow: 6px 6px 0px var(--text-color); background: var(--light-bg);">
    <h3 style="margin-top: 0; font-family: Georgia, serif; font-style: italic;">The Old-School Way</h3>
    <p>We evaluate the soil, lay down a proper base, pour it smooth, and cure it right. A straightforward process with no hidden surprises.</p>
  </div>
</div>

Ready to talk about your yard? Give us a shout and we'll come take a look.

[Get a Free Quote](/contact/){: .btn}
