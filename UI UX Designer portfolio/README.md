# Shreya Shake - UX/UI Portfolio Website

A modern, responsive portfolio website built with **Bootstrap 5**, custom CSS, and JavaScript. This site showcases a UX/UI designer's work, experience, skills, and testimonials with professional images integrated throughout.

## Features

✅ **Fully Responsive** - Mobile, tablet, and desktop optimized  
✅ **Dark Theme** - Modern dark design with neon yellow and cyan accents  
✅ **Professional Images** - High-quality images from Unsplash integrated throughout  
✅ **Bootstrap 5** - Built with Bootstrap for reliable responsive grid  
✅ **Interactive Features**:
   - Smooth scroll navigation with active link highlighting
   - Form validation and submission feedback
   - Project filtering (All, Mobile, Web, Logo)
   - Animated elements on scroll
   - Hover effects on cards and exhibits
   - Lazy loading image animations

✅ **Multiple Sections**:
- Navigation with sticky header
- Hero section with professional profile image and CTA buttons
- "Beyond the Interface" section with design philosophy image
- Experience timeline with 4 roles
- Tools & Skills showcase (11 tools with icons)
- Featured projects/exhibits with professional project images
- Client testimonials with star ratings
- Contact form with validation
- Footer with social links

## File Structure

```
UI UX Designer portfolio/
├── index.html          # Main HTML file with all content
├── styles.css          # Custom styling (800+ lines)
├── script.js           # JavaScript for interactivity
└── README.md          # This file
```

## Image Sources

All images are sourced from **Unsplash** (free, high-quality stock photos):

### Images Included:
1. **Profile Image** (Hero Section)
   - Professional portrait
   - URL: `https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=400&h=500&fit=crop`
   - Usage: Designer profile picture

2. **Design Philosophy Image** (About Section)
   - UX/UI Design workspace
   - URL: `https://images.unsplash.com/photo-1552664730-d307ca884978?w=600&h=400&fit=crop`
   - Usage: Visual representation of design philosophy

3. **SaaS Automation Project** (Exhibits)
   - Web design workspace
   - URL: `https://images.unsplash.com/photo-1561070791-2526d30994b5?w=600&h=450&fit=crop`
   - Usage: Featured SaaS automation platform project

4. **Mobile App Project** (Exhibits)
   - Mobile app design
   - URL: `https://images.unsplash.com/photo-1512941691920-25bda36a555f?w=600&h=450&fit=crop`
   - Usage: Featured financial app UI project

## Getting Started

### Option 1: Open in VS Code (Recommended for Development)
1. Open the folder in VS Code
2. Install the **Live Server** extension (by Ritwick Dey)
3. Right-click `index.html` → "Open with Live Server"
4. The site will open in your browser and auto-refresh on changes

### Option 2: Direct Browser Access (Quickest)
1. Double-click `index.html` to open in your default browser
2. Or drag and drop the file into your browser
3. **Note:** Requires internet connection for Unsplash images

### Option 3: Local Server (Full Featured)
```bash
# Using Python 3
python -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js (if installed)
npx http-server

# Using Live Server extension in VS Code
```
Then visit `http://localhost:8000`

## JavaScript Features

The included `script.js` file provides:

### 1. **Navigation Highlighting**
   - Active link shows current section
   - Auto-updates on scroll
   - Smooth anchor navigation

### 2. **Form Validation**
   - Client-side validation for contact form
   - Email format checking
   - Success/warning notifications
   - Auto-clearing after submission

### 3. **Project Filtering**
   - Filter exhibits by category (All, Mobile, Web, Logo)
   - Dynamic filtering functionality

### 4. **Scroll Animations**
   - Cards fade in as they enter viewport
   - Smooth scroll behavior across browser
   - Lazy loading for images

### 5. **Interactive Hover Effects**
   - Exhibit cards scale and move on hover
   - Smooth transitions throughout
   - Mobile-friendly touch support

## Customization Guide

### Change Colors
Edit the CSS variables in `styles.css`:
```css
:root {
    --primary-bg: #0a0e27;        /* Main background */
    --highlight-yellow: #d4ff00;  /* Yellow accent */
    --highlight-cyan: #00d4ff;    /* Cyan accent */
    --text-light: #ffffff;        /* Text color */
    --text-muted: #a0aec0;        /* Muted text */
}
```

### Replace Images
To use your own images, update the `src` URLs in `index.html`:

```html
<!-- Hero section profile image -->
<img src="your-image.jpg" alt="Profile" class="profile-img">

<!-- Philosophy/about section image -->
<img src="design-philosophy.jpg" alt="Design Philosophy" class="philosophy-img">

<!-- Project exhibit images -->
<img src="project-1.jpg" alt="Project Name" class="exhibit-img">
```

### Update Content
- **Name/Branding**: Edit "SHREYA SHAKE" in navbar and footer
- **Hero text**: Modify the heading and subtitle in the hero section
- **Experience**: Update years and titles in the experience cards
- **Skills**: Add/remove tool icons using Font Awesome icons
- **Testimonials**: Replace with actual client quotes
- **Contact info**: Update email and location
- **Social links**: Add your actual social media URLs

### Customize Project Images
You can:
1. **Use images from Unsplash**: Browse and replace URLs
   - https://unsplash.com - Free high-quality images
   
2. **Use local images**: Save to your folder and use relative paths
   ```html
   <img src="images/my-project.jpg" alt="Project" class="exhibit-img">
   ```

3. **Use other services**:
   - Pexels: https://www.pexels.com
   - Pixabay: https://pixabay.com
   - Shutterstock, Getty Images, etc.

### Font Awesome Icons
The site uses Font Awesome 6.4.0 icons. 

Browse available icons at: https://fontawesome.com/icons

To change an icon:
```html
<i class="fas fa-pen-fancy"></i>  <!-- Change to any Font Awesome icon -->
```

### Add More Sections
Copy and paste existing section patterns (like `exhibits-section`) and customize:
1. Copy the HTML structure
2. Update the content
3. Maintain the CSS class names for styling

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Android)
- Internet Explorer: Not supported (modern browsers only)

## Performance Tips

1. **Optimize images before replacing**:
   - Compress PNG/JPG files
   - Use WebP format for modern browsers
   - Target image size: 600-800px width

2. **Lazy load images for better performance**:
   ```html
   <img src="image.jpg" loading="lazy" alt="Description">
   ```

3. **Cache optimization**:
   - Browser caches external CSS/JS from CDN
   - Minify CSS/JS for production
   - Use service worker for offline support

4. **Image optimization tools**:
   - TinyPNG/TinyJPG - Online image compression
   - Squoosh - Google's image compressor
   - ImageOptim - Mac image optimization

## Deployment Options

### Netlify (Recommended - Free)
1. Push files to GitHub
2. Connect repo to Netlify
3. Auto-deploys on push
4. Free SSL certificate
5. CDN included

### Vercel
1. Push to GitHub
2. Import project in Vercel dashboard
3. Auto-deploys
4. Excellent performance

### GitHub Pages
1. Push to GitHub repo
2. Enable GitHub Pages in repo settings
3. Select main branch as source
4. Free hosting

### Traditional Hosting (GoDaddy, Bluehost, etc.)
1. Upload files via FTP to your hosting
2. Access via your domain
3. Full control over server

### Firebase Hosting
1. Install Firebase CLI
2. Initialize Firebase in project folder
3. Deploy with `firebase deploy`
4. Fast CDN distribution

## Dependencies

- **Bootstrap 5.3.0** - CSS framework (via CDN)
- **Font Awesome 6.4.0** - Icon library (via CDN)
- **Unsplash API** - Free image service (via CDN)
- **No build tools required** - Ready to use immediately

All external dependencies are loaded via CDN, so no `npm install` or build process needed.

## SEO Optimization

For better search engine visibility, add these to your HTML `<head>`:

```html
<meta name="description" content="UX/UI Designer Portfolio - Professional design services and case studies">
<meta name="keywords" content="UX Designer, UI Design, Product Design, User Experience">
<meta name="author" content="Your Name">
<meta property="og:title" content="Your Portfolio Title">
<meta property="og:description" content="Your portfolio description">
<meta property="og:image" content="your-image-url.jpg">
```

## Analytics

Add Google Analytics to track visitors:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_ID');
</script>
```

Replace `GA_ID` with your Google Analytics ID.

## Troubleshooting

| Issue | Solution |
|-------|----------|
| **Images not showing** | Check internet connection (CDN required). Try refreshing browser. |
| **Styling looks off** | Clear browser cache (Ctrl+Shift+Delete). Check that styles.css is in same folder. |
| **Form not working** | Form currently shows demo notifications. Add backend service (Formspree, Netlify Forms) to process submissions. |
| **JavaScript errors** | Check browser console (F12 → Console). Ensure script.js is linked in HTML. |
| **Navigation not highlighting** | Ensure section IDs match nav link href values. |
| **Images pixelated** | Use higher resolution images or add `loading="lazy"` attribute. |

## Enhancement Ideas

1. ✅ **Add smooth scroll** - Already enabled
2. ⚪ **Form backend** - Add Formspree or Netlify Forms
3. ⚪ **Dark mode toggle** - Add theme switcher
4. ⚪ **Analytics** - Add Google Analytics
5. ⚪ **SEO optimization** - Add meta tags
6. ⚪ **Accessibility** - Enhance alt text and ARIA labels
7. ⚪ **Blog section** - Add case studies
8. ⚪ **Animation library** - Integrate AOS or GSAP
9. ⚪ **Contact CMS** - Integrate backend
10. ⚪ **Multi-language** - Add i18n support

## Connect Form to Backend

To make the contact form actually send emails, you can use:

### Option 1: Formspree (Free)
1. Go to https://formspree.io
2. Create an account
3. Get your form endpoint
4. Update HTML:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" class="contact-form">
```

### Option 2: Netlify Forms (Free on Netlify)
1. Deploy to Netlify
2. Add `netlify` attribute to form:
```html
<form name="contact" method="POST" netlify class="contact-form">
```

### Option 3: EmailJS (Free tier available)
```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/index.min.js"></script>
<script>
  emailjs.init('YOUR_PUBLIC_KEY');
  document.querySelector('.contact-form').addEventListener('submit', function(e) {
    e.preventDefault();
    emailjs.sendForm('service_id', 'template_id', this);
  });
</script>
```

## License

Free to use and modify for your portfolio. No attribution required.

## Support & Resources

**Documentation:**
- Bootstrap: https://getbootstrap.com/docs/5.3/
- Font Awesome: https://fontawesome.com/docs/
- MDN Web Docs: https://developer.mozilla.org/

**Image Resources:**
- Unsplash: https://unsplash.com
- Pexels: https://www.pexels.com
- Pixabay: https://pixabay.com

**Tools:**
- VS Code: https://code.visualstudio.com/
- Chrome DevTools: Press F12 in Chrome
- Can I Use: https://caniuse.com/

---

**Ready to launch?** 🚀 Open `index.html` in your browser to see your professional portfolio live!

For questions or updates, check the official documentation links above or deploy to Netlify/Vercel for instant hosting.

