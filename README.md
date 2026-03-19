# Grace Alele — Personal Academic Website

Personal website of **Grace Ojemerenvhie Alele**, clinical AI researcher focused on medical imaging, AI safety, and equitable diagnostics in low-resource settings.

🌐 **Live site:** [gracealele.io](https://gracealele.io)

---

## About

This is the source code for my personal academic website. It showcases my research, publications, projects, and background. The site is built with plain HTML, CSS, and vanilla JavaScript — no frameworks, no build tools.

---

## Features

- **Research & Publications** — listing of papers, manuscripts, and conference posters
- **Projects** — showcase of AI/ML and software projects with links to code and data
- **News/Highlights** — timeline of recent research activity
- **Dark/Light mode** — toggle with persistent icon state
- **Scroll animations** — lightweight IntersectionObserver-based entrance animations
- **Expandable sections** — news, publications, conferences, and projects collapse by default with show more/less toggle
- **Personal section** — hobbies, teaching philosophy, and daily life log
- **Responsive design** — mobile and desktop layouts

---

## Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 (custom properties, flexbox, grid) |
| Scripting | Vanilla JavaScript (ES6+) |
| Icons | Font Awesome 6 |
| Hosting | — |

---

## Project Structure

```
├── index.html              # Main page
├── style.css               # Global styles
├── script.js               # All JS (theme, toggles, animations)
├── images/                 # Images and videos used across the site
├── data/                   # PDFs (papers, posters, CV)
└── pages/
    ├── blog.html           # Daily life log
    ├── woodworking.html    # Woodworking creative projects
    └── footwear.html       # Footwear design projects
```

---

## Running Locally

No build step required. Just clone and open:

```bash
git clone https://github.com/gracealele/gracealele.io.git
cd gracealele.io
open index.html
```

Or use a local server for best results:

```bash
# Python
python -m http.server 8000

# Node
npx serve .
```

Then visit `http://localhost:8000` in your browser.

---

## Customisation

All toggle thresholds (how many items show by default) are controlled in `initToggleSections()` inside `script.js`:

```javascript
// Change the number to control how many items show before "more" button
if (index >= 5) ...   // News: shows 5
if (index >= 3) ...   // Publications: shows 3
if (index >= 1) ...   // Conferences: shows 1
if (index >= 4) ...   // Projects: shows 4
```

Theme defaults to `light`. To change, update `data-theme` on the `<body>` tag in `index.html`.

---

## License

MIT License — see [LICENSE](./LICENSE) for details.

---

## Contact

- **Email:** alelegrace@gmail.com
- **Website:** [gracealele.io](https://gracealele.io)
- **LinkedIn:** [Grace Alele](https://linkedin.com/in/gracealele)
- **GitHub:** [gracealele](https://github.com/gracealele)
- **ORCID:** [Grace Alele](https://orcid.org/your-orcid-here)
