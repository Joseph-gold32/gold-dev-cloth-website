# GOLD & DEV — Modern Wardrobe Co.

A modern fashion storefront and brand website for curated clothing, skincare, and everyday luxury essentials.

## Overview

GOLD & DEV is a boutique-style fashion brand website created to showcase premium collections, editorial storytelling, and customer-first shopping experiences. The project is built as a responsive static website and is designed to work well on both desktop and mobile devices.

## Features

- Responsive landing page and product layout
- Mobile-friendly hamburger navigation
- Fashion and skincare product collection sections
- Story, blog, contact, and sign-in pages
- Clean static architecture for GitHub Pages deployment

## Project Structure

```text
GOLD-DEV PROJECT/
├── .github/
│   └── workflows/
│       └── deploy-pages.yml
├── assets/
│   ├── css/
│   │   └── main.css
│   ├── images/
│   └── js/
├── index.html
├── men.html
├── skin.html
├── story.html
├── contact.html
├── blog.html
├── auth.html
├── README.md
├── ORGANIZATION.md
├── SETUP_GUIDE.md
├── package.json
├── .gitignore
├── .nojekyll
├── TODO.md
└── index-responsive.html
```

## Local Development

Open the site directly in a browser, or run a local server:

```bash
py -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## GitHub Pages Deployment

This project is configured for deployment as a static website on GitHub Pages.

### Steps to publish

1. Push the repository to GitHub.
2. Open the repository on GitHub.
3. Go to Settings → Pages.
4. In the Source section, choose GitHub Actions.
5. Save the setting.

The workflow file in `.github/workflows/deploy-pages.yml` will build and publish the site automatically.

## Notes

- `index.html` is the homepage.
- The project uses static HTML, CSS, and JavaScript.
- Firebase/Auth code is used in the authentication pages when enabled.

## License

This project is intended for personal portfolio and brand showcase use.

## Contact

Joseph Gold
- GitHub: https://github.com/Joseph-gold32
- Project: https://github.com/Joseph-gold32/gold-dev-cloth-website
