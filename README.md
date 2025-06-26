# Diaspora Connect

Diaspora Connect is a web platform designed to help Kenyans living abroad (especially in America) access essential services in Kenya. The platform offers a wide range of services including legal assistance, document processing, healthcare, education support, property management, travel arrangements, and more.

## Features
- Service request forms for various needs (legal, travel, property, education, etc.)
- Responsive, mobile-friendly design
- Modern, accessible UI
- Fast, static site for easy deployment

## Project Structure
```
assets/   # Images, icons, and manifest
css/      # Stylesheets (main and form-specific)
js/       # JavaScript for interactivity
pages/    # HTML pages for each service
```

## Setup & Usage
1. **Clone or download the repository.**
2. **Open `pages/index.html` in your browser** to view the homepage.
3. **Navigate to other services** via the homepage or directly open any HTML file in the `pages/` directory.
4. **Forms** are powered by [Formspree](https://formspree.io/) for demo purposes. Update the form action URLs for production use.

## Image Optimization
For best performance, compress large images in the `assets/` folder. See below for optimization tips.

## Accessibility & SEO
- All pages use semantic HTML and descriptive alt text for images.
- Add or update meta tags for SEO (see below for recommendations).

## Contributing
Feel free to fork and submit pull requests for improvements!

---

### Recommended Meta Tags for SEO
```
<meta name="description" content="Diaspora Connect helps Kenyans in America access legal, travel, property, and other services in Kenya. Reliable, fast, and personal support.">
<meta name="keywords" content="Kenya, diaspora, services, legal, travel, property, education, healthcare, support">
<meta property="og:title" content="Diaspora Connect">
<meta property="og:description" content="Connecting Kenyans in America to Home. Trusted partner for car hire, property, travel, and more in Kenya.">
<meta property="og:image" content="/assets/SS2.png">
<meta property="og:type" content="website">
<meta property="og:url" content="https://yourdomain.com/">
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Diaspora Connect">
<meta name="twitter:description" content="Connecting Kenyans in America to Home. Trusted partner for car hire, property, travel, and more in Kenya.">
<meta name="twitter:image" content="/assets/SS2.png">
```

---

### Folder Structure Recommendation (for scaling)
```
css/
  styles.css
  form.css
  components/
    navbar.css
    footer.css
js/
  script.js
  modules/
    form-handler.js
    analytics.js
```

---

### Image Optimization Command (for Windows, using PowerShell & ImageMagick)
```
# Install ImageMagick if not already installed
# Then run this in the assets directory:
Get-ChildItem *.png | ForEach-Object { magick $_.FullName -strip -resize 1200x1200\> -quality 85 $_.FullName }
```
Or use an online tool like [Squoosh](https://squoosh.app/) for manual optimization.

---

### Accessibility & Responsiveness Checklist
- Use semantic HTML elements (`<header>`, `<main>`, `<nav>`, `<footer>`, etc.)
- All images have descriptive `alt` attributes
- Forms use `<label>` for all inputs
- Sufficient color contrast for text
- Test with keyboard navigation
- Responsive layouts using CSS Grid/Flex and media queries
- Viewport meta tag is present: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`

---

### License
MIT License 