
# The Research Paper Toolbox (COM 421 Project 1)

This starter implements a **sustainable information structure** for a module-based instructional site.

## Structure

```
research-paper-toolbox/
├── index.html
├── css/
│ └── screen.css
├── modules/
│ ├── topic.html
│ ├── research.html
│ └── data.html (placeholder page, prevents dead links)
└── assets/
├── icons/
│ └── hammer.svg
└── images/
└── illustrations/ (module figures live here)
├── ebsco_results.jpg
├── datalesson_raw.png
├── datalesson_binary.png
└── datalesson_descstats.png
```

## How to add a new module

1. Copy `modules/template.html` to `modules/module-N.html`.
2. Replace titles, headings, and content. Keep heading hierarchy.
3. Add links to figures in `/assets/images/` and write meaningful `alt` text.
4. Update the top navigation in `index.html` (and other pages if desired).
5. Validate HTML at <https://validator.w3.org/> and test keyboard navigation.

## Accessibility & Sustainability

- Semantic landmarks: `header`, `nav`, `main`, `article`, `section`, `footer`
- Skip link, proper heading order, high contrast, large click targets
- Single CSS file, no inline styles, minimal image weight

## Publish (GitHub Pages)

- Create a repo (e.g., `research-paper-toolbox`), push this folder.
- In repo settings → Pages → Deploy from branch → `main` → `/root`.
- Your site will be available at `https://<username>.github.io/research-paper-toolbox/`.

## Self-critique

- **Structure:** Semantic landmarks on every page; consistent top nav; active tab marked with `aria-current="page"`.
- **Accessibility:** Skip link, logical heading order, meaningful `alt` text; decorative logo uses `alt=""` + `aria-hidden`.
- **Sustainability:** Single shared CSS; relative paths only; clear modules directory; template page for quick expansion.
- **Quality checks:** All pages pass the W3C validator (no errors). Verified 200s for HTML/CSS/images in DevTools → Network.
- **Tradeoffs:** Chose simple, readable typography and minimal visuals over heavier styling to keep focus on content.
- **Next steps:** Add print styles + dark mode, small design-token system, breadcrumbs/site map, and complete placeholder modules.