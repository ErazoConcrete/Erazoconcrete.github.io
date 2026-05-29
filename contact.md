---
layout: default
title: Contact & Quote Request
---

<div class="hero">
  <h1>Get Your Free Quote</h1>
  <p>Contact us today for a professional consultation and estimate</p>
</div>

## Quick Contact Info

**Phone:** [{{ site.phone }}](tel:{{ site.phone | remove: ' ' | remove: '(' | remove: ')' | remove: '-' }})  
**Email:** [{{ site.email }}](mailto:{{ site.email }})

---

## Quote Request Form

Fill out the form below with your project details. We'll review your request and get back to you within 24 hours with a professional estimate.

<form name="quote-request" method="POST" action="https://formspree.io/f/xkoeeobg" class="quote-form">
  
  <div class="form-group">
    <label for="name">Your Name *</label>
    <input type="text" id="name" name="name" required>
  </div>

  <div class="form-group">
    <label for="email">Email Address *</label>
    <input type="email" id="email" name="email" required>
  </div>

  <div class="form-group">
    <label for="phone">Phone Number *</label>
    <input type="tel" id="phone" name="phone" required>
  </div>

  <div class="form-group">
    <label for="service">Service Type *</label>
    <select id="service" name="service" required>
      <option value="">-- Select a Service --</option>
      <option value="Foundation Work">Foundation Work</option>
      <option value="Concrete Driveway">Concrete Driveway</option>
      <option value="Loading Dock">Loading Dock</option>
      <option value="Concrete Slab">Concrete Slab</option>
      <option value="Site Preparation">Site Preparation</option>
      <option value="Parking Lot">Parking Lot</option>
      <option value="Custom Project">Custom Project</option>
      <option value="Other">Other</option>
    </select>
  </div>

  <div class="form-group">
    <label for="project-details">Project Details *</label>
    <textarea id="project-details" name="message" placeholder="Describe your project, any specific requirements, measurements, or questions..." required></textarea>
  </div>

  <div class="form-group">
    <label for="timeline">Preferred Timeline</label>
    <select id="timeline" name="timeline">
      <option value="">-- No preference --</option>
      <option value="ASAP">ASAP</option>
      <option value="Within 2 weeks">Within 2 weeks</option>
      <option value="Within 1 month">Within 1 month</option>
      <option value="Flexible">Flexible</option>
    </select>
  </div>

  <div class="form-group">
    <label for="budget">Estimated Budget (Optional)</label>
    <input type="text" id="budget" name="budget" placeholder="e.g., $5,000 - $10,000">
  </div>

  <div class="form-group">
    <label for="attachments">Attach Files (Optional)</label>
    <p style="font-size: 0.9em; color: #7f8c8d; margin-bottom: 10px;">Upload plans, diagrams, photos, or other documents (PDF, PNG, JPG, DOC, etc.)</p>
    <input type="file" id="attachments" name="attachments" multiple accept=".pdf,.png,.jpg,.jpeg,.gif,.doc,.docx,.xls,.xlsx,.dwg">
  </div>

  <button type="submit" class="btn">Send Quote Request</button>

</form>

---

## What Happens Next?

1. **Submit Your Details** - Fill out the form with your project information
2. **Quick Review** - We review your request and project scope
3. **Contact You** - We'll call or email within 24 hours
4. **Free Consultation** - Discuss your project and needs in detail
5. **Detailed Quote** - Receive a professional estimate with timeline

## Why Choose Erazo Concrete?

- **Professional Team** - Experienced concrete specialists
- **Free Consultation** - No obligation initial assessment
- **Competitive Pricing** - Fair, transparent quotes
- **Quality Guarantee** - 100% satisfaction on all work
- **Fast Response** - 24-hour quote turnaround
