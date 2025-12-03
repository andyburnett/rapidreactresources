# Rapid React Resources - Static Website

A clean, modern static website for serving game resources, manuals, and PDF documents to the public.

## Project Structure

```
rapidreactresources/
├── public/                 # HTML files served to the web
│   ├── index.html         # Welcome/home page
│   ├── game-manual.html   # Game manual page
│   ├── documents.html     # Documents library page
│   └── about.html         # About page
├── docs/                  # PDF documents
│   ├── game-manual.pdf
│   ├── quick-start.pdf
│   ├── strategy-guide.pdf
│   ├── setup-instructions.pdf
│   ├── faq.pdf
│   └── house-rules.pdf
├── css/                   # Stylesheets
│   └── style.css         # Main stylesheet with responsive design
└── README.md             # This file
```

## Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Clean Navigation**: Fixed sidebar menu for easy access to all pages
- **Document Library**: Organized section for PDF documents and resources
- **Modern Styling**: Professional appearance with smooth transitions and hover effects
- **Accessible**: Semantic HTML and proper navigation structure
- **SEO Friendly**: Proper meta tags and page structure

## Pages

### Home (index.html)
Welcome page with quick links to main sections and overview cards.

### Game Manual (game-manual.html)
Comprehensive guide covering:
- Getting started
- Basic rules
- Game mechanics
- Strategies and tips
- FAQ
- PDF download option

### Documents Library (documents.html)
Grid-based document browser with downloadable PDFs for:
- Game Manual
- Quick Start Guide
- Strategy Guide
- Setup Instructions
- FAQ Document
- House Rules

### About (about.html)
Information about the project, mission, community involvement, and support options.

## Deployment Options

### Static Hosting (Recommended)
1. **GitHub Pages** (Free)
   - Push to `gh-pages` branch
   - Enable Pages in repository settings

2. **Netlify** (Free tier available)
   - Connect your repository
   - Auto-deploys on push

3. **Vercel** (Free tier available)
   - Connect your repository
   - Automatic deployments

4. **Amazon S3 + CloudFront**
   - Upload `public/` and `css/` folders
   - Perfect for high-traffic public distribution

### Local Development
Simply open `public/index.html` in your browser or use a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx http-server public/

# Using PHP
php -S localhost:8000 -t public/
```

## Adding PDF Documents

Place PDF files in the `docs/` folder and create links in the appropriate pages:

```html
<a href="../docs/your-document.pdf" class="btn">Download PDF</a>
```

## Customization

### Change Colors
Edit `css/style.css` and modify the color variables in the sidebar and accent colors:
- Primary color: `#2c3e50` (dark blue-gray)
- Accent color: `#3498db` (bright blue)

### Add More Pages
1. Create a new HTML file in `public/`
2. Copy the structure from an existing page
3. Add a new menu item in the `<nav class="sidebar-nav">` section on all pages

### Update Navigation
Edit the `<nav class="sidebar-nav">` section on all pages to add/remove menu items.

## Browser Support

- Chrome/Edge (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Mobile browsers

## License

Content is provided under Creative Commons Attribution 4.0 International License. See LICENSE file for details.

## Contributing

Community contributions are welcome! To contribute:
1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## Support

For questions or issues, please create an issue in the repository.
