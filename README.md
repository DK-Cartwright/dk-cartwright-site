# DK Cartwright LLC - Static Website

A clean, modern static website for DK Cartwright LLC, converted from Wix to be deployable on GitHub Pages.

## Overview

This website showcases web design and development services, featuring:

-   Professional homepage with company information
-   Portfolio section displaying completed projects
-   Contact form for client inquiries
-   Responsive design that works on all devices
-   Clean, modern UI with fast loading times

## Project Structure

```
├── css/
│   └── styles.css          # Main stylesheet
├── index.html              # Homepage (clean version)
├── portfolio.html          # Portfolio page (clean version)
├── contact.html            # Contact page (clean version)
├── Wix Projects Collection.csv  # Project data from original site
├── README.md               # This file
└── [original files]        # Original Wix-generated files (for reference)
```

## Features

### Homepage (`index.html`)

-   Hero section with call-to-action
-   Services overview
-   About section
-   Professional branding

### Portfolio (`portfolio.html`)

-   Project showcase with details
-   Technology stack information
-   Client information
-   Direct links to live projects
-   Projects include:
    -   What'sUp 24/7 (Laravel)
    -   Payroc (dotCMS)
    -   Taylor University (dotCMS)
    -   Hamilton, IN (Wix)
    -   Library History Database (React/Golang)
    -   Hamilton Eyecare Center (WordPress)
    -   And more...

### Contact (`contact.html`)

-   Comprehensive contact form
-   Project type selection
-   Budget and timeline options
-   Form validation
-   Process overview

## Technologies Used

-   **HTML5** - Semantic markup
-   **CSS3** - Modern styling with Flexbox and Grid
-   **JavaScript** - Form validation and interactivity
-   **Responsive Design** - Mobile-first approach
-   **GitHub Pages** - Static site hosting

## Deployment on GitHub Pages

### Option 1: Automatic Deployment

1. Push this repository to GitHub
2. Go to repository Settings
3. Scroll to "Pages" section
4. Select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"
7. Your site will be available at `https://[username].github.io/[repository-name]`

### Option 2: Custom Domain

1. Follow steps 1-6 above
2. Add a `CNAME` file with your custom domain
3. Configure DNS settings with your domain provider
4. Enable "Enforce HTTPS" in GitHub Pages settings

## File Replacement Guide

To complete the conversion:

1. **Backup originals** (already done - they're preserved)
2. **Replace files**:
    ```bash
    mv index_new.html index.html
    mv portfolio_new.html portfolio.html
    mv contact_new.html contact.html
    ```
3. **Test locally** (optional):
    ```bash
    # Using Python 3
    python3 -m http.server 8000
    # Then visit http://localhost:8000
    ```

## Contact Form Setup

The contact form currently shows a success message. To make it functional:

### Option 1: Formspree (Recommended for GitHub Pages)

1. Sign up at [Formspree.io](https://formspree.io)
2. Create a new form
3. Replace the form action in `contact.html`:
    ```html
    <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST"></form>
    ```

### Option 2: Netlify Forms

1. Deploy to Netlify instead of GitHub Pages
2. Add `netlify` attribute to form:
    ```html
    <form netlify name="contact"></form>
    ```

### Option 3: Custom Backend

-   Set up a server-side script (PHP, Node.js, etc.)
-   Configure email sending
-   Add proper validation and security

## Performance Optimizations

-   Minified CSS (can be further optimized)
-   Semantic HTML for better SEO
-   Responsive images (add when images are included)
-   Fast loading times
-   Mobile-optimized design

## Browser Support

-   Chrome (latest)
-   Firefox (latest)
-   Safari (latest)
-   Edge (latest)
-   Mobile browsers

## Development

### Local Development

```bash
# Clone the repository
git clone [repository-url]
cd dk-cartwright

# Start local server
python3 -m http.server 8000
# or
npx serve .
```

### Making Changes

1. Edit HTML/CSS files
2. Test locally
3. Commit and push to GitHub
4. Changes will automatically deploy to GitHub Pages

## Migration Notes

### Removed from Original Wix Site

-   Wix-specific JavaScript bundles
-   Wix tracking and analytics code
-   Wix-specific meta tags
-   Heavy framework dependencies
-   Wix image hosting dependencies

### Added for Static Site

-   Clean, semantic HTML structure
-   Custom CSS with modern features
-   Responsive design
-   Form validation
-   SEO-friendly markup
-   Fast loading performance

## Next Steps

1. **Replace original files** with new clean versions
2. **Set up contact form** with preferred service
3. **Add analytics** (Google Analytics, etc.)
4. **Optimize images** if adding project screenshots
5. **Test thoroughly** across devices and browsers
6. **Deploy to GitHub Pages**

## Support

For questions about this conversion or deployment, please refer to:

-   [GitHub Pages Documentation](https://docs.github.com/en/pages)
-   [Formspree Documentation](https://help.formspree.io/)
-   [Web Development Best Practices](https://web.dev/)

---

**DK Cartwright LLC** - Professional Web Design & Development
