# Personal Portfolio - Vanilla HTML/CSS/JavaScript

A modern, responsive personal portfolio website built with pure HTML, CSS, and JavaScript. No frameworks or build tools required!

## Features

✨ **Modern Design**
- Beautiful gradient hero section with animated background
- Clean, professional layout with smooth scrolling
- Responsive design that works on all devices
- Professional typography with Playfair Display and Inter fonts

🌙 **Dark Mode**
- Toggle between light and dark themes
- Theme preference saved to localStorage
- Smooth transitions between themes
- Perfect contrast ratios for accessibility

📱 **Responsive & Mobile-Friendly**
- Mobile hamburger menu
- Touch-friendly navigation
- Optimized for all screen sizes
- Fast loading times

🎨 **Interactive Elements**
- Smooth scroll navigation
- Hover effects and animations
- Contact form with validation
- Scroll-to-top button
- Active navigation highlighting

⚡ **Performance**
- No dependencies or build tools
- Lightweight CSS (21KB)
- Minimal JavaScript (11KB)
- Fast page load times
- Optimized images

## Project Structure

```
portfolio_vanilla/
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # All styling with dark mode support
├── js/
│   └── script.js       # All JavaScript functionality
├── images/
│   ├── hero-bg.jpg     # Hero section background
│   ├── projects-bg.jpg # Projects section images
│   └── skills-bg.jpg   # Skills section background
└── README.md           # This file
```

## Getting Started

### Quick Start
1. Open `index.html` in your web browser
2. That's it! No installation or build process needed

### Local Development Server
If you want to run a local server:

**Using Python 3:**
```bash
cd portfolio_vanilla
python3 -m http.server 8000
# Visit http://localhost:8000
```

**Using Node.js (http-server):**
```bash
npm install -g http-server
cd portfolio_vanilla
http-server
```

**Using PHP:**
```bash
cd portfolio_vanilla
php -S localhost:8000
```

## Customization

### Update Your Information

1. **Name & Title** - Edit the hero section in `index.html`
2. **About Section** - Update the about text and highlights
3. **Projects** - Replace project cards with your own work
4. **Skills** - Update skill categories and items
5. **Contact Info** - Add your email, phone, and social links
6. **Colors** - Modify CSS variables in `css/styles.css`

### CSS Variables (Theming)

Edit the color scheme in `css/styles.css`:

```css
:root {
    --primary-color: #2563eb;      /* Main blue color */
    --text-primary: #1a1a1a;       /* Dark text */
    --bg-primary: #ffffff;         /* White background */
    /* ... more variables */
}

body.dark-mode {
    --primary-color: #3b82f6;      /* Lighter blue for dark mode */
    --text-primary: #e2e8f0;       /* Light text */
    --bg-primary: #0f172a;         /* Dark background */
    /* ... more variables */
}
```

### Add Your Own Images

1. Replace images in the `images/` folder
2. Update image paths in `index.html`
3. Optimize images for web (use tools like TinyPNG)

## Features Explained

### Dark Mode
- Click the moon/sun icon in the navigation to toggle dark mode
- Your preference is saved in browser localStorage
- Smooth CSS transitions between themes

### Navigation
- Smooth scrolling to sections
- Active link highlighting
- Mobile hamburger menu
- Sticky navigation bar

### Contact Form
- Built-in form validation
- Success/error notifications
- Responsive design
- Ready to integrate with backend

### Scroll-to-Top Button
- Appears after scrolling 300px down
- Smooth scroll back to top
- Mobile-friendly

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Metrics

- **Page Load Time**: < 2 seconds
- **Lighthouse Score**: 90+
- **File Sizes**:
  - HTML: ~24KB
  - CSS: ~21KB
  - JavaScript: ~11KB
  - Images: ~300KB

## Accessibility

- Semantic HTML structure
- ARIA labels for interactive elements
- Keyboard navigation support
- Color contrast compliance
- Mobile accessibility optimized

## SEO Optimization

- Meta tags for description
- Semantic HTML
- Proper heading hierarchy
- Mobile-responsive
- Fast loading times

## Deployment

### GitHub Pages
1. Push to GitHub repository
2. Enable GitHub Pages in settings
3. Your portfolio is live!

### Netlify
1. Connect your GitHub repository
2. Netlify auto-deploys on push
3. Free HTTPS included

### Traditional Hosting
1. Upload files via FTP
2. No build process needed
3. Works on any web server

## Customization Tips

1. **Change Primary Color**: Update `--primary-color` in CSS
2. **Add More Sections**: Copy existing section structure
3. **Modify Fonts**: Update Google Fonts link in HTML
4. **Add Animations**: Extend CSS animations
5. **Integrate Backend**: Connect contact form to email service

## Common Customizations

### Add a Blog Section
```html
<section id="blog" class="blog">
    <div class="container">
        <h2 class="section-title">Latest Articles</h2>
        <!-- Add blog posts here -->
    </div>
</section>
```

### Connect Contact Form
Replace the form submission handler in `script.js`:
```javascript
// Send to your backend/email service
fetch('/api/contact', {
    method: 'POST',
    body: JSON.stringify(formData)
})
```

### Add Google Analytics
Add this to `index.html` before closing `</head>`:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'GA_ID');
</script>
```

## License

Free to use for personal and commercial projects.

## Support

For questions or issues:
1. Check the code comments
2. Review CSS variables for styling
3. Inspect JavaScript functions for functionality

## Version History

- **v1.0** - Initial release with all core features

---

Made with ❤️ for developers who love clean, simple code.
