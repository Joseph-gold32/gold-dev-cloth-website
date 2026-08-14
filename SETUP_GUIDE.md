# 🚀 GOLD & DEV - Quick Setup Guide

## Overview
Your GOLD-DEV project has been reorganized for better structure and responsive mobile design. This guide helps you get started immediately.

---

## ✨ What Was Improved

### ✅ Before (Old Structure)
```
GOLD-DEV PROJECT/
├── index.html
├── men.html
├── skin.html
├── contact.html
├── story.html
├── blog.html
├── auth.html
├── style.css
├── sign.css
└── projects/
```
❌ **Problems:** Files everywhere, hard to navigate, not properly organized

### ✅ After (New Structure)
```
GOLD-DEV PROJECT/
├── index.html
├── assets/
│   ├── css/
│   │   └── main.css (NEW - Enhanced responsive)
│   ├── images/
│   └── js/
├── pages/
│   ├── men.html
│   ├── skin.html
│   ├── contact.html
│   ├── story.html
│   ├── blog.html
│   └── auth.html
└── projects/
```
✅ **Benefits:** Clean, organized, professional, easy to scale

---

## 🎯 What You Need to Do Now

### Step 1: Update HTML Files in `pages/` Folder
Your old HTML files still exist at the root. You need to move them to the `pages/` folder.

**Files to move:**
- `men.html` → `pages/men.html`
- `skin.html` → `pages/skin.html`
- `contact.html` → `pages/contact.html`
- `story.html` → `pages/story.html`
- `blog.html` → `pages/blog.html`
- `auth.html` → `pages/auth.html`

**How to do it in VS Code:**
1. Drag and drop each file into the `pages` folder, OR
2. Cut (Ctrl+X) each file and paste (Ctrl+V) in `pages` folder

### Step 2: Update CSS Links in All HTML Files
**For files in `pages/` folder, change:**
```html
<!-- OLD -->
<link rel="stylesheet" href="./style.css">

<!-- NEW -->
<link rel="stylesheet" href="../assets/css/main.css">
```

**For index.html (already done):**
```html
<link rel="stylesheet" href="./assets/css/main.css">
```

### Step 3: Update Internal Navigation Links
**In `pages/men.html`, `pages/skin.html`, etc.:**
```html
<!-- OLD -->
<a href="./index.html">Home</a>
<a href="./contact.html">Contact</a>

<!-- NEW -->
<a href="../index.html">Home</a>
<a href="./contact.html">Contact</a>
```

### Step 4: Test Everything
- Open `index.html` in browser
- Click navigation links - should work
- Check that styles load (should look good)
- Test on mobile phone screen

---

## 📱 Mobile Responsiveness Guide

### Your CSS Now Supports:
- **Phones (320px - 767px)** - Mobile-first design
- **Tablets (768px - 1023px)** - Balanced layouts
- **Desktops (1024px+)** - Full features

### Test Responsive Design:
1. Open `index.html` in Chrome/Firefox
2. Press `F12` to open Developer Tools
3. Click device icon (top left) or press `Ctrl+Shift+M`
4. Drag to resize - watch layout adapt!

### Key Mobile Features:
```
✅ Hamburger menu on phones
✅ 2-column product grid on mobile
✅ 3-column on tablet
✅ 4-column on desktop
✅ Touch-friendly buttons
✅ Readable text at all sizes
```

---

## 🎨 Using the New CSS

### Main CSS File Location
```
assets/css/main.css
```

### Key Features:
```css
/* Mobile-first approach */
.element {
  font-size: 14px;  /* Mobile size */
}

@media (min-width: 768px) {
  .element {
    font-size: 18px;  /* Tablet size */
  }
}

@media (min-width: 1024px) {
  .element {
    font-size: 24px;  /* Desktop size */
  }
}
```

### Modify Colors:
Find this section in `assets/css/main.css`:
```css
:root {
  --cream: #faf6ef;
  --ink: #211d19;
  --gold: #b3874f;        /* Change this! */
  --gold-deep: #8f6a38;
  /* ... more colors ... */
}
```

---

## 📝 Editing Your Content

### Homepage
Edit `index.html` for:
- Hero section text
- Product cards
- Footer links

### Other Pages
Edit files in `pages/` folder:
- `men.html` - Men's collection
- `skin.html` - Skin care products
- `contact.html` - Contact form
- `story.html` - Company story
- `blog.html` - Blog posts
- `auth.html` - Login/Registration

---

## 🔗 Important Path References

### From Root (index.html)
```html
<link rel="stylesheet" href="./assets/css/main.css">
<a href="./pages/men.html">Men</a>
```

### From Pages Folder (pages/men.html)
```html
<link rel="stylesheet" href="../assets/css/main.css">
<a href="../index.html">Home</a>
<a href="./contact.html">Contact</a>
```

---

## 🧪 Quick Testing

### Test in Browser
```bash
# Option 1: Direct open
open index.html

# Option 2: Local server (better)
python -m http.server 8000
# Visit: http://localhost:8000
```

### Test Mobile View
```
1. Open DevTools (F12)
2. Click device toggle (or Ctrl+Shift+M)
3. Select "iPhone X" or similar
4. See mobile layout
5. Toggle between orientations
```

---

## 📊 File Structure Checklist

- [ ] `index.html` exists and loads CSS correctly
- [ ] `assets/css/main.css` exists
- [ ] `pages/` folder exists
- [ ] All `.html` files moved to `pages/` folder
- [ ] CSS links updated in all moved files
- [ ] Navigation links working from all pages
- [ ] Styles display correctly on mobile
- [ ] No broken links or 404 errors

---

## 🐛 Troubleshooting

### Styles not showing?
- Check browser cache (Ctrl+Shift+Delete)
- Verify CSS path is correct
- Open DevTools → Network tab to see if CSS loads

### Navigation links broken?
- Check path starts with `../` if in pages folder
- Check path starts with `./` if in root folder
- Use relative paths, not absolute paths

### Mobile view looks wrong?
- Open DevTools (F12)
- Check responsive mode (Ctrl+Shift+M)
- Verify viewport meta tag exists:
  ```html
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  ```

---

## 💡 Pro Tips

### 1. Use a Local Server
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js
npx http-server
```

### 2. Keep Mobile First
When adding new CSS:
- Write mobile styles first
- Add `@media (min-width: ...)` for larger screens

### 3. Test Different Devices
- iPhone SE (375px)
- iPhone 12 (390px)
- iPad (768px)
- Desktop (1440px)

### 4. Use Browser DevTools
- F12 to open DevTools
- Ctrl+Shift+M for responsive mode
- Throttle network in DevTools → Network tab

---

## 📚 Next Steps

1. **Move all HTML files to `pages/` folder**
2. **Update CSS links** in moved files
3. **Test everything** on mobile and desktop
4. **Optimize images** (resize and compress)
5. **Add your products** and content
6. **Deploy to hosting** (Netlify, Vercel, etc.)

---

## 📞 Quick Reference

| Need to... | File Location |
|-----------|---------------|
| Change colors | `assets/css/main.css` (Line 1-20) |
| Edit homepage | `index.html` |
| Edit men's page | `pages/men.html` |
| Add products | Edit respective page |
| Change logo | Edit SVG in HTML |
| Update footer | Bottom of `index.html` |

---

## ✅ Verification Checklist

**Before deployment, verify:**

- [ ] All navigation links work
- [ ] CSS loads on all pages
- [ ] Mobile view looks correct
- [ ] Tablet view looks correct
- [ ] Desktop view looks correct
- [ ] All images display properly
- [ ] No console errors (DevTools)
- [ ] All paths are relative (not absolute)

---

**Status:** ✅ Ready to Use  
**Last Updated:** August 14, 2024  
**Created for:** GOLD & DEV Project

