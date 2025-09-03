# Changelog Component

A responsive, accessible **Changelog timeline** built with **HTML + CSS (Flexbox)**, based on the project brief from [roadmap.sh](https://roadmap.sh/projects/changelog-component).

> Replace placeholders like `YOUR_GH_USERNAME` and `YOUR_NAME` before publishing.

![Preview](./preview.png)

---

## Live Demo

**URL:** https://YOUR_GH_USERNAME.github.io/changelog-component

---

## Project Page URL

- Roadmap project: https://roadmap.sh/projects/changelog-component

---

## Features

- Semantic HTML (`<ol>`, `<li>`, `<time>`) for accessibility and SEO
- Three-column Flexbox layout: **date • line/dot • content**
- Mobile responsive layout that collapses elegantly on small screens
- CSS variables, rounded card style, and tasteful hover states
- Dark mode support via `prefers-color-scheme`
- Zero JavaScript

---

## Tech

- HTML5
- CSS3 (Flexbox)

---

## Structure

```
.
├── index.html
├── styles.css
└── README.md
```

- **index.html** – header, timeline, and CTA button
- **styles.css** – variables, timeline line and dots, responsive rules

---

## Getting Started (Local)

1. **Create repo** on GitHub and clone it
   ```bash
   git clone https://github.com/YOUR_GH_USERNAME/changelog-component.git
   cd changelog-component
   ```
2. **Copy files** into the repo (index.html, styles.css, README.md).
3. **Open** `index.html` in a browser  
   - Double-click the file, or  
   - Use VS Code Live Server for auto-reload.

> No dependencies, build steps, or package managers required.

---

## Deploy to GitHub Pages

1. Commit and push your code to `main`:
   ```bash
   git add .
   git commit -m "feat: initial changelog component"
   git push origin main
   ```
2. Go to **Settings → Pages**.
3. Under **Source**, select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **Save**.  
   Your site will shortly be available at:
   ```
   https://YOUR_GH_USERNAME.github.io/changelog-component
   ```

---

## Add or Update Entries

Each change is an `<li>` in the ordered list:

```html
<ol class="timeline">
  <li class="timeline__item">
    <time datetime="2024-09-03" class="timeline__date">September 3, 2024</time>
    <div class="timeline__dot" aria-hidden="true"></div>
    <div class="timeline__content">
      <h3 class="timeline__title">Announcing Projects on Frontend Roadmap</h3>
      <p class="timeline__desc">Short summary of the change.</p>
    </div>
  </li>
</ol>
```

Keep the ISO date in `datetime` and human-friendly text in the element body.

---

## Accessibility

- Use `<time datetime="YYYY-MM-DD">` for machine-readable dates.
- The vertical line is decorative and implemented with a CSS pseudo-element.
- Color contrast meets WCAG AA in both light and dark modes.

---

## Submitting Your Solution (roadmap.sh)

1. Make the repo **public** and verify the **Live Demo** URL.
2. Include this README with the **project page URL**.
3. Submit your solution on the roadmap project page to get community feedback.

---

## License

MIT © Yana Makogon
