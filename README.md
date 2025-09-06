# NestQuest Landing Page

A modern, responsive landing page for NestQuest - the privacy-first baby tracking and family wellness app.

## Features

- **Responsive Design** - Looks great on all devices
- **Modern Animations** - Smooth scroll effects and interactive elements
- **Privacy-Focused Messaging** - Highlights NestQuest's key differentiators
- **Clean Code** - Semantic HTML, organized CSS, vanilla JavaScript
- **Performance Optimized** - Fast loading, minimal dependencies

## File Structure

```
nestquest-landing/
├── index.html          # Main HTML file
├── styles.css          # All CSS styles
├── script.js           # JavaScript functionality
├── README.md           # This file
└── _redirects          # Netlify redirects (optional)
```

## Quick Start

1. **Local Development**
   ```bash
   # Navigate to the directory
   cd nestquest-landing
   
   # Open in browser (or use a local server)
   open index.html
   
   # Or use Python's built-in server
   python3 -m http.server 8000
   # Then visit http://localhost:8000
   ```

2. **Deploy to Netlify**
   - Drag and drop the entire folder to [Netlify Drop](https://app.netlify.com/drop)
   - Or connect your Git repository for automatic deployments

## Customization

### Adding Real Screenshots
Replace the placeholder phone mockups in `index.html`:
```html
<!-- Replace this placeholder -->
<div class="phone-placeholder">
    <ion-icon name="phone-portrait-outline"></ion-icon>
    <p>App Screenshot</p>
    <small>Replace with actual screenshot</small>
</div>

<!-- With actual image -->
<img src="path/to/screenshot.png" alt="NestQuest App Screenshot">
```

### Updating Colors
The app uses NestQuest's brand colors defined in `styles.css`:
```css
/* Primary brand colors */
--primary: #9C27B0;      /* Rich Purple */
--secondary: #A78BFA;    /* Light Purple */
--accent: #C4B5FD;       /* Very Light Purple */

/* Dark mode colors */
--primary-dark: #6366F1; /* Indigo */
--secondary-dark: #4F46E5; /* Darker Indigo */
```

### Adding Background Images
If you have background assets, add them to an `images/` folder and update the CSS:
```css
.hero {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%),
                url('images/your-background.jpg');
    background-size: cover;
    background-position: center;
}
```

### Email Signup Integration
Update the email signup in `script.js` to connect to your email service:
```javascript
// Replace the simulation with actual API call
fetch('/api/subscribe', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ email: email })
})
```

## Deployment Options

### Netlify (Recommended)
1. **Drag & Drop**: Visit [netlify.com/drop](https://app.netlify.com/drop) and drag the folder
2. **Git Integration**: Connect your repository for automatic deployments
3. **Custom Domain**: Add your domain in Netlify's domain settings

### Other Platforms
- **Vercel**: `npx vercel --prod`
- **GitHub Pages**: Push to a repository and enable Pages
- **Firebase Hosting**: `firebase deploy`

## Performance Tips

- **Images**: Optimize screenshots with tools like TinyPNG
- **Fonts**: Consider using system fonts for faster loading
- **CDN**: Use a CDN for Ionicons if needed for better caching

## Browser Support

- Chrome/Edge 88+
- Firefox 85+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Content Sections

1. **Hero** - Main value proposition and CTA
2. **Features** - Six key features with icons
3. **App Preview** - Screenshots/mockups of the app
4. **Testimonials** - Social proof (placeholder content)
5. **Download** - App store buttons and email signup
6. **Footer** - Links and legal pages

## Next Steps

1. **Add Real Content**
   - Replace placeholder testimonials with real user feedback
   - Add actual app screenshots
   - Update app store links when available

2. **SEO Optimization**
   - Add meta tags for social sharing
   - Create sitemap.xml
   - Add structured data markup

3. **Analytics**
   - Add Google Analytics or similar
   - Set up conversion tracking for email signups

4. **Legal Pages**
   - Create privacy policy page
   - Add terms of service
   - Set up contact form

## Support

For questions about the landing page, contact the development team or create an issue in the repository.

---

Built with ❤️ for NestQuest families
