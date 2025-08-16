# Professional Product Designer Portfolio

A beautiful, modern, and responsive portfolio website designed for product designers. Features a sleek dark/light mode design, multilingual support (English/Portuguese), and smooth animations.

## 🌟 Features

### Design & UX
- **Modern Dark/Light Mode**: Elegant theme switching with smooth transitions
- **Responsive Design**: Fully responsive across all devices (desktop, tablet, mobile)
- **Smooth Animations**: Subtle animations and transitions for enhanced user experience
- **Professional Typography**: Inter and Space Grotesk fonts for optimal readability
- **Accessibility**: WCAG compliant with keyboard navigation and screen reader support

### Multilingual Support
- **English (EN)**: Primary language
- **Portuguese (PT-BR)**: Complete translation
- **Easy Language Toggle**: One-click language switching
- **Persistent Settings**: Language preference saved in localStorage

### Sections
1. **Hero Section**: Eye-catching introduction with call-to-action buttons
2. **About/Resume**: Professional background with interactive timeline
3. **Skills**: Visual grid of design tools, UX skills, and soft skills
4. **Projects**: Featured case studies with detailed modal views
5. **Contact**: Contact form with social media links

### Interactive Features
- **Sticky Navigation**: Smooth scrolling with active section highlighting
- **Project Modals**: Detailed case study views with project information
- **Contact Form**: Functional form with validation and notifications
- **Mobile Menu**: Hamburger menu for mobile devices
- **Scroll Effects**: Fade-in animations on scroll

## 🚀 Quick Start

### Prerequisites
- A modern web browser
- Basic knowledge of HTML, CSS, and JavaScript (for customization)

### Installation

1. **Clone or Download**
   ```bash
   git clone <repository-url>
   cd portfolio_project
   ```

2. **Open the Website**
   - Simply open `index.html` in your web browser
   - Or use a local server for development:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js (if you have http-server installed)
     npx http-server
     ```

3. **View the Website**
   - Navigate to `http://localhost:8000` (if using a server)
   - Or open `index.html` directly in your browser

## 🎨 Customization Guide

### Personal Information

#### Update Basic Info
Edit `index.html` and replace the placeholder content:

```html
<!-- Update your name -->
<span class="hero-name">Your Name</span>

<!-- Update your title -->
<span class="hero-tagline" data-lang="hero-tagline">Product Designer</span>

<!-- Update your description -->
<p class="hero-description" data-lang="hero-description">
    Your custom description here...
</p>
```

#### Update Experience Timeline
In the About section, modify the timeline items:

```html
<div class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
        <h4 class="timeline-role">Your Job Title</h4>
        <p class="timeline-company">Company Name • 2022 - Present</p>
        <p class="timeline-description" data-lang="timeline-1">Your job description</p>
    </div>
</div>
```

#### Update Skills
Modify the skills section to match your expertise:

```html
<div class="skill-item">
    <div class="skill-icon">🎨</div>
    <span class="skill-name">Your Skill</span>
</div>
```

#### Update Projects
1. **Project Cards**: Modify the project cards in the HTML
2. **Project Data**: Update the `projectData` object in `script.js`
3. **Project Images**: Replace SVG placeholders with actual project images

### Styling Customization

#### Colors
Modify the CSS custom properties in `styles.css`:

```css
:root {
    --accent-color: #00d4ff;        /* Primary accent color */
    --bg-primary: #1a1a1a;          /* Main background */
    --text-primary: #f8f8f8;        /* Primary text color */
    /* ... other colors */
}
```

#### Typography
Update font imports in `index.html`:

```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">
```

#### Spacing & Layout
Adjust spacing variables in `styles.css`:

```css
:root {
    --space-xs: 0.5rem;    /* Extra small spacing */
    --space-sm: 1rem;      /* Small spacing */
    --space-md: 1.5rem;    /* Medium spacing */
    --space-lg: 2rem;      /* Large spacing */
    --space-xl: 3rem;      /* Extra large spacing */
    --space-2xl: 4rem;     /* 2X large spacing */
    --space-3xl: 6rem;     /* 3X large spacing */
}
```

### Content Management

#### Adding New Languages
1. Add translations to the `translations` object in `script.js`:

```javascript
const translations = {
    en: { /* English translations */ },
    pt: { /* Portuguese translations */ },
    es: { /* Spanish translations */ }
};
```

2. Update the language toggle in `index.html`:

```html
<button class="language-toggle" id="language-toggle">
    <span data-lang="lang-en">EN</span>
    <span data-lang="lang-pt">PT</span>
    <span data-lang="lang-es">ES</span>
</button>
```

#### Adding New Projects
1. Add project card to HTML
2. Add project data to `projectData` object in `script.js`
3. Update project images and descriptions

#### Social Media Links
Update the social media links in the contact section:

```html
<a href="https://linkedin.com/in/yourprofile" class="social-link" target="_blank" rel="noopener">
    <!-- LinkedIn icon -->
</a>
```

## 📱 Responsive Design

The website is fully responsive with breakpoints at:
- **Desktop**: 1024px and above
- **Tablet**: 768px - 1023px
- **Mobile**: Below 768px

### Mobile Features
- Hamburger menu navigation
- Optimized touch targets
- Simplified layouts for small screens
- Mobile-first animations

## 🔧 Technical Details

### File Structure
```
portfolio_project/
├── index.html          # Main HTML file
├── styles.css          # All CSS styles
├── script.js           # JavaScript functionality
├── README.md           # This file
└── favicon.ico         # Website icon (optional)
```

### Browser Support
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### Performance Features
- Optimized CSS with CSS custom properties
- Debounced scroll events
- Lazy loading for animations
- Minimal JavaScript footprint
- Efficient DOM manipulation

### SEO Features
- Semantic HTML structure
- Meta tags for social sharing
- Proper heading hierarchy
- Alt text for images
- Open Graph tags

## 🎯 Best Practices

### Content Guidelines
- Keep descriptions concise and impactful
- Use action verbs in project descriptions
- Include measurable outcomes
- Maintain consistent tone across languages

### Image Guidelines
- Use high-quality images (minimum 1200px width)
- Optimize images for web (compress without losing quality)
- Use descriptive alt text
- Consider loading performance

### Performance Tips
- Compress images before uploading
- Minimize external dependencies
- Use web fonts efficiently
- Test on various devices and browsers

## 🚀 Deployment

### GitHub Pages
1. Push your code to a GitHub repository
2. Go to repository Settings > Pages
3. Select source branch (usually `main`)
4. Your site will be available at `https://username.github.io/repository-name`

### Netlify
1. Drag and drop your project folder to Netlify
2. Or connect your GitHub repository
3. Your site will be deployed automatically

### Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your project directory
3. Follow the prompts to deploy

## 🔍 Troubleshooting

### Common Issues

**Language not switching**
- Check that all elements have proper `data-lang` attributes
- Verify translations exist in the `translations` object

**Theme not persisting**
- Ensure localStorage is enabled in your browser
- Check for JavaScript errors in the console

**Mobile menu not working**
- Verify all JavaScript files are loaded
- Check for CSS conflicts

**Images not loading**
- Ensure image paths are correct
- Check file permissions
- Verify image formats are supported

### Performance Issues
- Optimize images using tools like TinyPNG
- Minimize external requests
- Use browser dev tools to identify bottlenecks

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📞 Support

If you need help customizing or deploying your portfolio:

1. Check the troubleshooting section above
2. Review the customization guide
3. Open an issue in the repository
4. Contact the developer

## 🎨 Credits

- **Fonts**: Inter and Space Grotesk from Google Fonts
- **Icons**: Custom SVG icons and emoji
- **Design**: Modern, clean design principles
- **Inspiration**: Best practices from leading design portfolios

---

**Happy designing! 🎨✨**
