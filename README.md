# GOLD & DEV — Modern Wardrobe Co.

A modern fashion e-commerce brand built by **Joseph Gold**, featuring collections for women, men, and skincare products.

## Brand Overview

GOLD & DEV is a thoughtfully designed clothing and skincare brand offering:
- **Womenswear** — Clean silhouettes, honest fabrics, timeless pieces
- **Menswear** — Tailored fits, quality construction, versatile layers
- **Skincare** — Vegan, dermatologist-tested, clean luxury formulations
- **The Journal** — Stories on craft, style, and the making of Gold & Dev

## Pages

| Page | File | Description |
|------|------|-------------|
| Home (Women) | `index.html` | Women's collection landing page with hero, products, testimonials |
| Men | `men.html` | Men's collection with video hero, product grid, brand film |
| Skincare | `skin.html` | Skincare products with glow routine, categories, reviews |
| Story | `story.html` | Brand origin story, timeline, values, maker film |
| Contact | `contact.html` | Contact form, FAQ, studio info |
| Blog | `blog.html` | The Journal — articles on craft, style, interviews |
| Auth | `auth.html` | Sign in / Sign up with Firebase authentication |

## Tech Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **Authentication:** Firebase Auth (Email/Password + Google)
- **Hosting:** GitHub Pages

## Firebase Configuration

The site uses Firebase Authentication. To configure for your own Firebase project:

1. Go to [Firebase Console](https://console.firebase.google.com)
2. Create or select your project
3. Enable **Email/Password** and **Google** sign-in methods
4. Update `firebaseConfig` in `auth.html` with your project credentials
5. Add your GitHub Pages domain to **Authorized domains** in Firebase Auth settings

## Local Development

Simply open any `.html` file in your browser. For Firebase features (auth), use a local server:

```bash
# Using Python
python -m http.server 8000
# Or with VS Code Live Server extension
```

## Deployment

The site is deployed on **GitHub Pages** from the `main` branch root.

---

© 2026 GOLD & DEV. Built by Joseph Gold.
</｜｜DSML｜｜parameter>
</create_file>
