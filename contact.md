---
layout: default
title: Get a Quote
---

<section class="page-hero" style="display: flex; flex-direction: column; justify-content: center; min-height: 250px;">
  <div class="page-hero-content">
    <h1>Contact Erazo Concrete</h1>
    <p>Connect with us for a fast quote request and project review.</p>
  </div>
</section>

<section class="contact-quote">
  <div class="content-panel">
    <h2>Request a Quote</h2>
    <p>Tell us about your project and we’ll respond with a quote and next steps.</p>
  </div>
</section>

<section class="contact-details">
  <div class="content-panel" id="contact-form">
    <h2>Send a Message</h2>
    <form action="https://formspree.io/f/xkoeeobg" method="POST">
      <!-- Redirects to your custom Thank You page after submission -->
      <input type="hidden" name="_next" value="https://erazoconcrete.github.io/thanks/">
      <div class="form-group">
        <label for="name">Name</label>
        <input type="text" id="name" name="name" placeholder="Your Name" required>
      </div>
      <div class="form-group">
        <label for="email">Email</label>
        <input type="email" id="email" name="email" placeholder="Your Email" required>
      </div>
      <div class="form-group">
        <label for="phone">Phone</label>
        <input type="tel" id="phone" name="phone" placeholder="Your Phone Number">
      </div>
      <div class="form-group">
        <label for="message">Project Details</label>
        <textarea id="message" name="message" placeholder="Briefly describe your project" rows="5" required></textarea>
      </div>
      <button type="submit" class="btn">Submit Request</button>
    </form>
  </div>

  <div class="content-panel contact-office">
    <h2>Office Details</h2>
    <p><strong>Phone:</strong> <a href="tel:3392317006">339 231 7006</a></p>
    <p><strong>Email:</strong> <a href="mailto:estimating@erazoconcrete.com">estimating@erazoconcrete.com</a></p>
    <!-- Placeholder for your new Google Business link. Replace the # below with your new URL when ready! -->
    <a href="#" target="_blank" rel="noopener noreferrer">
      <img src="/assets/LOGOTIPO-Sien-FONDO.jpeg" alt="Erazo Concrete Logo" class="contact-logo" style="margin-top: 20px; max-width: 100%; border-radius: 25px; -webkit-mask-image: radial-gradient(ellipse at center, black 50%, transparent 100%); mask-image: radial-gradient(ellipse at center, black 50%, transparent 100%);">
    </a>
  </div>
</section>
