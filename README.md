# Jacken Mendoza — About Me

> A responsive, single-page student portfolio built with semantic HTML and modern CSS.

<p align="center">
  <img src="images/profile.png" alt="Jacken Mendoza" width="180">
</p>

<p align="center">
  <strong>Personal introduction · interests · academic path · skills · goals</strong>
</p>

<p align="center">
  <a href="#getting-started">Getting started</a> ·
  <a href="#project-highlights">Highlights</a> ·
  <a href="#customization">Customization</a> ·
  <a href="#credits">Credits</a>
</p>

---

## About the project

This website is Jacken Ismael C. Mendoza's personal **CS101 final project** for Bicol University College of Science. It introduces Jacken as a first-year BS Computer Science student and presents his interests, journey into computing, developing skills, future goals, and personal reflection.

The page is intentionally lightweight: it uses only HTML and CSS, so it can be opened locally without installing packages, configuring a build tool, or running a backend.

## Project highlights

### A clear visual identity

The design uses a calm, Coolors-inspired palette:

| Color     | Role                             | Hex       |
| --------- | -------------------------------- | --------- |
| Navy      | Primary text and contrast        | `#0A1A2F` |
| Blue      | Links, actions, and emphasis     | `#0066FF` |
| Sky blue  | Supporting accent                | `#38A3FF` |
| Teal      | Secondary accent                 | `#2EC4B6` |
| Mint      | Soft palette finish              | `#9BE8C8` |
| Off-white | Surfaces and section backgrounds | `#F3F6FB` |

### Content sections

The sticky navigation provides quick access to:

- **Hello** — quick facts and a personal summary
- **About** — interests and conversation topics
- **My Path** — the story behind choosing Computer Science
- **Skills** — favorite website and current technical skills
- **Goals** — academic, career, and family goals
- **Reflection** — lessons learned while building the project

### Responsive and accessible by default

- Uses semantic elements including `nav`, `header`, `main`, `section`, `figure`, `details`, and `footer`.
- Includes descriptive image alternative text, a page description, keyboard focus outlines, and a labeled navigation landmark.
- Uses responsive breakpoints for tablets and phones.
- Respects `prefers-reduced-motion` by disabling animations for visitors who request less motion.
- Uses a system-font stack, so there are no external font requests.

## Getting started

### Option 1: Open the file directly

1. Download or clone this repository.
2. Open `index.html` in a browser.

### Option 2: Run a local server

From the project directory, use any static file server. For example, with Python installed:

```bash
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000) in your browser.

> No package installation or build step is required.

## File structure

```text
Mendoza-Jacken-ITC-Webpage/
├── index.html              # Page content and semantic structure
├── style.css               # Theme, layout, responsive rules, and animations
├── images/
│   └── profile.png         # Profile photo used in the hero section
└── README.md               # Project documentation
```

## How it works

```text
index.html
    │
    ├── Sticky navigation ── jumps to section IDs
    ├── Hero ─────────────── profile, introduction, actions, trait palette
    └── Main content ─────── facts, interests, path, skills, goals
             │
             └── style.css ── tokens → layout → components → responsive rules
```

The stylesheet is organized in layers:

1. **Design tokens** — colors, typography, spacing behavior, and easing.
2. **Page foundations** — box sizing, body width, links, and focus states.
3. **Components** — navigation, hero, buttons, palette, panels, cards, table, tags, and footer.
4. **Responsive rules** — one-column panels and touch-friendly navigation below `800px` and `500px`.
5. **Motion preferences** — reduced-motion overrides for accessibility.

## Customization

### Update personal content

Edit the text and links in [index.html](index.html). The most common updates are:

- Replace the profile image or `alt` text.
- Update the hero introduction and navigation labels.
- Add or remove interests, skills, and goals.
- Change the GitHub profile URL.
- Update the footer course or school information.

### Change the theme

The main colors and font stack live at the top of [style.css](style.css) inside `:root`. Updating the custom properties there changes the visual theme consistently across the page:

```css
:root {
  --text: #0a1a2f;
  --blue: #0066ff;
  --soft: #f3f6fb;
}
```

### Add another section

1. Add a navigation link whose `href` matches a unique section `id`.
2. Add a new `<section class="panel" id="your-section">` inside `<main>`.
3. Keep the existing heading and content order so the responsive grid continues to work.

## Browser support

The page uses broadly supported HTML and CSS features, including Flexbox, Grid, CSS custom properties, `clamp()`, `backdrop-filter`, and the native `details` element. The scroll-linked reveal animation is progressive enhancement: browsers that do not support it still display the content normally.

For best results, use a current version of Chrome, Edge, Firefox, or Safari.

## Quality checklist

Before publishing a customized version:

- [ ] Check every navigation link and external URL.
- [ ] Confirm the profile image still loads and has useful alternative text.
- [ ] Test the page at desktop, tablet, and phone widths.
- [ ] Tab through the page to confirm focus indicators are visible.
- [ ] Check the page with reduced motion enabled.
- [ ] Proofread personal details, spelling, and course information.

## Credits

Created by **Jacken Ismael C. Mendoza** for **CS101 at Bicol University College of Science**.

Built with:

- HTML5
- CSS3
- A profile image stored locally in `images/`

## License

This is a personal educational project. The content and profile image are intended for this project and should not be reused without permission.

Claude Made this README.md with the help of my prompting.
