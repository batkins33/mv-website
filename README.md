# mv-website

Modern Vestige — Static site assets for curated vintage collectibles

## Overview

This repository serves as a static asset host for modernvestive.com, deployed and hosted via Netlify. It provides a centralized location for images, stylesheets, JavaScript files, and fonts that can be referenced by the main website.

## Repository Structure

```
mv-website/
├── public/                 # Public assets directory (served by Netlify)
│   ├── images/            # Image assets
│   ├── css/               # Stylesheets
│   ├── js/                # JavaScript files
│   ├── fonts/             # Custom fonts
│   └── index.html         # Landing page
├── netlify.toml           # Netlify configuration
└── README.md              # This file
```

## Usage

### Accessing Assets

Once deployed to Netlify, assets can be accessed via:

```
https://your-netlify-domain.netlify.app/images/your-image.jpg
https://your-netlify-domain.netlify.app/css/your-styles.css
https://your-netlify-domain.netlify.app/js/your-script.js
https://your-netlify-domain.netlify.app/fonts/your-font.woff2
```

### Adding New Assets

1. Place your assets in the appropriate directory under `public/`
2. Commit and push your changes
3. Netlify will automatically deploy the updates

## Deployment

This repository is configured to deploy automatically to Netlify:

- **Publish directory**: `public/`
- **Build command**: None required (static assets only)
- **Deploy**: Automatic on push to main branch

## Cache Strategy

Assets are served with optimized cache headers:
- Images, CSS, JS, and fonts: 1 year cache (immutable)
- Security headers enabled for all routes

## Contributing

When adding assets:
1. Ensure files are optimized (compressed images, minified CSS/JS)
2. Use meaningful, descriptive filenames
3. Update relevant documentation if needed

## License

All rights reserved - Modern Vestige
