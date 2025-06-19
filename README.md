# Modern Portfolio Website

A clean, minimalist portfolio website inspired by modern design principles. Features responsive design, smooth animations, and interactive elements.

## Features

- **Responsive Design**: Works perfectly on all devices
- **Modern UI**: Clean, minimalist design with smooth animations
- **Interactive Portfolio**: Filterable project gallery
- **Contact Form**: Functional contact form with validation
- **Smooth Scrolling**: Seamless navigation between sections
- **Mobile Menu**: Responsive hamburger navigation
- **Optimized Performance**: Fast loading with lazy loading images

## Structure

```
portfolio/
├── index.html          # Main HTML file
├── styles.css          # CSS styles
├── script.js           # JavaScript functionality
└── README.md          # This file
```

## Customization Guide

### 1. Personal Information

**Replace the following placeholders in `index.html`:**

- `YOUR NAME` → Your actual name
- `your.email@example.com` → Your email address
- `Your City, Your Country` → Your location
- Social media links (Instagram, LinkedIn, GitHub, Dribbble)

### 2. Content Updates

**Hero Section:**

- Update the greeting and description in the hero section
- Modify the subtitle to reflect your profession

**About Section:**

- Replace the about text with your personal story
- Update the skills list with your expertise
- Replace the placeholder image with your photo

**Portfolio Section:**

- Replace placeholder images with your actual project images
- Update project titles, descriptions, and links
- Modify categories in the filter buttons as needed

### 3. Styling Customization

**Colors (in `styles.css`):**

```css
:root {
  --primary-color: #000; /* Main brand color */
  --text-color: #333; /* Text color */
  --light-text: #666; /* Secondary text */
  --bg-color: #fff; /* Background color */
  --accent-color: #f5f5f5; /* Section backgrounds */
}
```

**Typography:**

- Font family: Currently using 'Inter' from Google Fonts
- You can change this in the CSS file

### 4. Adding Projects

To add a new project to the portfolio:

1. **Add HTML in the portfolio grid:**

```html
<div class="portfolio-item" data-category="your-category">
  <div class="portfolio-image">
    <img src="path-to-your-image.jpg" alt="Project Name" />
    <div class="portfolio-overlay">
      <h3>Project Name</h3>
      <p>Brief description</p>
      <a href="project-link" class="portfolio-link">View Project</a>
    </div>
  </div>
</div>
```

2. **Categories available:**
   - `web` - Web Design
   - `branding` - Branding
   - `development` - Development
   - Add custom categories by updating filter buttons

### 5. Contact Form

The contact form currently shows an alert on submission. To make it functional:

1. **For static hosting:** Use services like Formspree, Netlify Forms, or EmailJS
2. **For backend integration:** Connect to your server endpoint in `script.js`

**Example with Formspree:**

```html
<form
  id="contactForm"
  action="https://formspree.io/f/your-form-id"
  method="POST"
></form>
```

### 6. Images

**Recommended image sizes:**

- Hero/About photo: 300x400px
- Portfolio images: 400x300px
- Maintain aspect ratios for best results

**Image optimization:**

- Use WebP format for better performance
- Compress images before uploading
- Consider lazy loading (already implemented)

## Deployment

### Option 1: GitHub Pages

1. Create a GitHub repository
2. Upload your files
3. Enable GitHub Pages in repository settings
4. Your site will be available at `username.github.io/repository-name`

### Option 2: Netlify

1. Drag and drop your folder to Netlify
2. Get instant deployment with custom domain options

### Option 3: Vercel

1. Connect your GitHub repository
2. Automatic deployments on code changes

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Performance Tips

1. **Optimize Images**: Compress and use appropriate formats
2. **Minimize HTTP Requests**: Combine files when possible
3. **Use CDN**: For fonts and external libraries
4. **Enable Gzip**: On your server for faster loading

## Accessibility

The portfolio includes:

- Semantic HTML structure
- Alt text for images
- Keyboard navigation support
- Focus indicators
- Screen reader friendly elements

## License

This template is free to use for personal and commercial projects. No attribution required, but appreciated!

## Support

For questions or customization help:

- Create an issue in the repository
- Check the documentation
- Review the code comments

---

**Happy building! 🚀**
