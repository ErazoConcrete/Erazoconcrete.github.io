# Erazo Concrete LLC - Professional Website

A professional, fully-featured website for Erazo Concrete LLC built with Jekyll and hosted on GitHub Pages.

## ✨ Features

- **Professional Design** - Modern, responsive layout optimized for all devices
- **Service Pages** - Detailed information about each service offering
- **Project Portfolio** - Showcase completed projects with before/after details
- **Quote Request Form** - Integrated contact form with Formspree for lead capture
- **Mobile Responsive** - Beautiful on desktop, tablet, and mobile devices
- **SEO Optimized** - Built-in SEO tags and meta information
- **Easy Updates** - Simple markdown-based content management

## 📁 Website Structure

```
├── index.md                    # Home page
├── services.md                 # Services overview
├── about.md                    # About company
├── contact.md                  # Contact & quote form
├── projects.md                 # Projects portfolio
├── _services/                  # Individual service pages
│   ├── driveways.md
│   ├── patios.md
│   ├── foundation.md
│   └── repairs.md
├── _projects/                  # Project case studies
│   ├── modern-driveway.md
│   ├── luxury-patio.md
│   └── commercial-foundation.md
├── _layouts/                   # Custom HTML layouts
│   └── default.html
├── assets/css/                 # Styling
│   └── style.css
└── _config.yml                 # Jekyll configuration
```

## 🚀 Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/ErazoConcrete/Erazoconcrete.github.io.git
cd Erazoconcrete.github.io
```

### 2. Install Dependencies

```bash
bundle install
```

### 3. Run Locally

```bash
bundle exec jekyll serve
```

Visit `http://localhost:4000` in your browser.

## 📧 Setting Up Formspree (Quote Request Form)

The contact form uses **Formspree** to handle form submissions without needing a backend server.

### Steps:

1. **Go to Formspree**: Visit https://formspree.io/
2. **Sign Up**: Create a free account
3. **Create New Form**: Click "New Form"
4. **Configure Form**:
   - Project name: "Erazo Concrete Quote Requests"
   - Email: Your email address for receiving quotes
5. **Get Your Form ID**: After creating, you'll see your form ID (looks like: `f/xxxxxxxxx`)
6. **Update contact.md**:
   - Open `contact.md`
   - Find this line: `action="https://formspree.io/f/xyzabc123"`
   - Replace `xyzabc123` with your actual form ID
   - Save the file

### Example:
```html
<!-- Before -->
<form method="POST" action="https://formspree.io/f/xyzabc123">

<!-- After (with your ID) -->
<form method="POST" action="https://formspree.io/f/abcd1234efgh5678">
```

### Test the Form:
1. Fill out the form at `/contact/`
2. You should receive an email confirmation
3. Form submissions will be forwarded to your email

## 📝 Customization Guide

### Update Company Info

Edit `_config.yml`:

```yaml
title: Erazo Concrete LLC
description: Concrete services and solutions
author: Erazo Concrete LLC
email: your-email@example.com
phone: (555) 123-4567
url: https://erazo-concrete.com
```

### Add New Services

1. Create a new file in `_services/` folder (e.g., `stamped-concrete.md`)
2. Use this template:

```markdown
---
layout: default
title: Stamped Concrete
category: stamped
---

<div class="hero">
  <h1>🎨 Professional Stamped Concrete</h1>
  <p>Beautiful decorative finishes</p>
</div>

## Service Description

Your content here...

[Get a Quote](/contact/){: .btn}
```

3. The service automatically appears on the Services page!

### Add New Projects

1. Create a new file in `_projects/` folder (e.g., `backyard-stamped.md`)
2. Use this template:

```markdown
---
layout: default
title: Stunning Backyard Transformation
category: Patio
image: /assets/images/project-image.jpg
description: Beautiful stamped concrete patio
completed: "2025-12"
location: Downtown Area
client_name: Jane & Mike D.
---

## Project Overview

Your project details here...

> "Client testimonial quote here" - Client Name

[Get Started](/contact/){: .btn}
```

3. The project automatically appears on the Projects page!

### Add Project Images

1. Create `assets/images/` folder if it doesn't exist
2. Add your project images to this folder
3. Reference in project front matter: `image: /assets/images/your-image.jpg`

### Customize Colors & Styling

Edit `assets/css/style.css` and update these CSS variables:

```css
:root {
  --primary-color: #2c3e50;      /* Header background */
  --accent-color: #e74c3c;       /* Buttons & highlights */
  --light-bg: #ecf0f1;           /* Light backgrounds */
  --text-color: #2c3e50;         /* Body text */
  --text-light: #7f8c8d;         /* Light text */
}
```

## 📱 Navigation & Pages

The site automatically generates navigation from these pages:

- **Home** (`/`) - index.md
- **Services** (`/services/`) - services.md
- **Projects** (`/projects/`) - projects.md
- **About** (`/about/`) - about.md
- **Get Quote** (`/contact/`) - contact.md

## 🎯 Best Practices

### Content Tips

- Use clear, benefit-focused language
- Include specific project details and results
- Add client testimonials for social proof
- Keep photos/images to under 500KB each
- Update projects and testimonials regularly

### SEO Tips

- Each page has SEO tags (title, description, keywords)
- Use descriptive filenames and headings
- Include service keywords naturally
- Add meta descriptions to front matter

### Performance

- Optimize images before uploading
- Minimize CSS (already done)
- Keep content focused and scannable
- Use proper heading hierarchy

## 🔧 Troubleshooting

### Form not working?
- Verify Formspree form ID is correct in `contact.md`
- Check email is confirmed in Formspree account
- Test with your own email first

### Styling looks broken?
- Clear browser cache (Ctrl+Shift+Delete)
- Check CSS file is in `assets/css/style.css`
- Verify no CSS filename typos

### Navigation not appearing?
- Verify page has proper front matter (layout, title)
- Check file is in root directory (not in a folder)
- Rebuild with `bundle exec jekyll serve`

### Services/Projects not showing?
- Verify files are in `_services/` or `_projects/` folders
- Check YAML front matter is properly formatted
- Services need `category:` and Projects need `category:`, `description:`, `completed:`

## 📦 Deployment

The site automatically deploys to GitHub Pages when you push to main branch.

1. Push your changes:
```bash
git add .
git commit -m "Update content"
git push origin main
```

2. GitHub Pages automatically builds and publishes
3. Visit `https://erazoconcrete.github.io` to view live site

## 📄 License

This website is for Erazo Concrete LLC.

## 🤝 Support

For Jekyll documentation: https://jekyllrb.com/  
For Formspree help: https://formspree.io/help/  
For GitHub Pages: https://pages.github.com/
