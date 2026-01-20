# Noah Paladino - Personal Website

Modern, accessible portfolio website built with Jekyll and hosted on GitHub Pages.

## Features

### 🎨 Modern Design
- Clean, professional layout with modern color scheme
- Responsive design that works on all devices
- Smooth animations and hover effects
- WCAG AA compliant contrast ratios

### 📚 BibTeX Bibliography System
- Publications managed via `references.bib` file
- Automatic bibliography page generation
- Citation keys linked to research projects
- Easy to add and update publications

### 🏷️ Tag Filtering System
- Filter research and projects by tags
- Interactive tag buttons with smooth transitions
- Tags include: Machine Learning, Dark Matter, Data Acquisition, Hardware, Software, etc.
- Accessible with keyboard navigation and screen reader support

### ♿ Accessibility
- ARIA labels on all interactive elements
- Semantic HTML5 elements (section, article, nav)
- Screen reader announcements for dynamic content
- Keyboard navigation support
- High contrast ratios for text readability

### 📱 Responsive Design
- Mobile-first approach
- Works perfectly on phones, tablets, and desktops
- Touch-friendly buttons and controls

## Structure

```
.
├── _config.yml              # Site configuration and content
├── _includes/
│   ├── bibliography.html    # Bibliography rendering component
│   ├── head.html           # HTML head with meta tags and fonts
│   └── tags-filter.html    # Tag filtering component
├── _layouts/
│   └── default.html        # Default page layout
├── _sass/
│   ├── _variables.scss     # Design tokens and theme variables
│   ├── _modern-portfolio.scss  # Modern portfolio styles
│   ├── base.scss           # Base styles and imports
│   └── bootstrap/          # Bootstrap 5 framework
├── assets/
│   ├── css/style.css       # Compiled CSS
│   ├── img/                # Images
│   ├── pdf/                # PDF files (CV)
│   └── font-awesome/       # Icon fonts
├── index.html              # Homepage
├── publications.html       # Publications page
└── references.bib          # BibTeX file for publications
```

## Configuration

### Adding Research Entries

Edit `_config.yml` to add research projects:

```yaml
research:
  entries:
    - title: "Project Title"
      link: "https://project-url.com"
      timeline: "2024 - Present"
      tags:
        - "Machine Learning"
        - "Software"
      publications:
        - https://doi.org/...
      citation_keys:
        - citation_key_from_bibtex
      description: >-
        Project description goes here.
```

### Adding Publications

Edit `references.bib` to add publications:

```bibtex
@article{citation_key,
  title={Paper Title},
  author={Author, Name and Others},
  journal={Journal Name},
  year={2024},
  url={https://doi.org/...}
}
```

Then update `_includes/bibliography.html` to include the new publication in the JavaScript array.

### Customizing Colors

Edit `_sass/_variables.scss` to change the color scheme:

```scss
$primary-color: #2563eb;  // Main brand color
$primary-dark: #1e40af;   // Hover states
$primary-light: #60a5fa;  // Contrast on dark backgrounds
```

## Development

### Local Development

1. Install Jekyll and dependencies:
   ```bash
   gem install jekyll bundler
   ```

2. Run the development server:
   ```bash
   jekyll serve
   ```

3. Open http://localhost:4000 in your browser

### GitHub Pages

The site automatically deploys to GitHub Pages when changes are pushed to the main branch.

## Technologies

- **Jekyll** - Static site generator
- **Bootstrap 5** - CSS framework
- **Font Awesome** - Icons
- **Inter** - Modern typeface for headings
- **SCSS** - CSS preprocessing

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## License

All rights reserved © 2015-2026 Noah Paladino

## Credits

- Design: Noah Paladino
- Built with Jekyll
- Hosted on GitHub Pages
