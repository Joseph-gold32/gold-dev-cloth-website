# Gold & Dev Website — Responsive & Deployment Tasks

## Progress Tracker

### ✅ Completed
- [x] Analyzed all 7 pages and their CSS breakpoints
- [x] Verified GitHub repo setup (branch `main`, origin `Joseph-gold32/gold-dev-cloth-website`)
- [x] Set up git identity (Joseph Gold / joseph@golddev.com)

### ⬜ In Progress / To Do

#### Responsive Fixes
- [ ] **men.html** — Fix `filmVideo` JS reference (add missing `id="filmVideo"` to the film `<video>` element)
- [ ] **story.html** — Fix `heroVideo` / `filmVideo` JS references (add missing IDs); fix invalid Pexels video URL so hero video plays
- [ ] **skin.html** — Repair broken/truncated auth modal (re-add missing sign-in/sign-up forms inside the modal)
- [ ] Standardize brand naming to **GOLD & DEV** across pages (remove "Nova & Oak" / "ModernEssentials" leftovers)
- [ ] Fix `img{width:100%;height:100%}` distortion on layout images where needed
- [ ] Final responsive review of all breakpoints (320px–1024px) on every page

#### Hosting / Deployment
- [ ] Create `.github/workflows/deploy.yml` to auto-deploy to GitHub Pages on push to `main`
- [ ] Commit all changes
- [ ] Push to GitHub (triggers Pages build)
- [ ] Verify live site URL

#### Docs
- [ ] Update `README.md` with deployment status
- [ ] Update `TODO.md` notes

---

## Notes
- Hosting: **GitHub Pages** via GitHub Actions workflow (no `gh` CLI auth required).
- Site: `https://<owner>.github.io/<repo>/` after first successful deploy.
