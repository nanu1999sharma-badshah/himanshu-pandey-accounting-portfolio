# Himanshu Pandey · Animated Portfolio

[![Status](https://img.shields.io/badge/status-live-22c55e?style=for-the-badge)](https://claude.ai/artifact/8i4G5gBH6QPLgGRZVHSRjf)
[![Stack](https://img.shields.io/badge/stack-HTML%20%7C%20CSS%20%7C%20JS-8b5cf6?style=for-the-badge)](#tech-stack)
[![Dependencies](https://img.shields.io/badge/dependencies-zero-5eead4?style=for-the-badge)](#tech-stack)
[![License](https://img.shields.io/badge/license-all%20rights%20reserved-f472b6?style=for-the-badge)](#license)

A single-file, animated personal website built from my resume. It presents my work as an **Accounting Executive** in Accounts Receivable, Accounts Payable, bank and credit card reconciliation, intercompany accounting, and Oracle ERP Cloud.

**Live site:** [claude.ai/artifact/8i4G5gBH6QPLgGRZVHSRjf](https://claude.ai/artifact/8i4G5gBH6QPLgGRZVHSRjf)

---

## Contents

- [Highlights](#highlights)
- [Sections](#sections)
- [Animations and effects](#animations-and-effects)
- [Browser features used](#browser-features-used)
- [Tech stack](#tech-stack)
- [Getting started](#getting-started)
- [Customisation](#customisation)
- [Browser support](#browser-support)
- [Known limitations](#known-limitations)
- [Roadmap](#roadmap)
- [License](#license)

---

## Highlights

- **Scroll-driven reveals:** sections animate in as you scroll, each with its own entrance (slide, zoom, blur-to-sharp, 3D flip, or rise).
- **Animated hero:** each letter of the name flips into place, and the tagline types out and cycles through phrases.
- **Light and dark themes:** a toggle switches themes with a circular transition that grows from the click point.
- **Glass cards:** cards with a cursor-following spotlight, a glowing gradient border, 3D tilt, and a grid that dims the others on hover.
- **Responsive layout:** works from small phones to large desktops, with container-aware skill cards.
- **Survey form:** star rating, validation, and a modal thank-you message.
- **Reduced-motion support:** animations turn off for users who prefer less motion.

---

## Sections

| Section | Anchor | Content |
| :--- | :--- | :--- |
| Hero | `#top` | Name, role, typewriter tagline, and calls to action |
| About | `#about` | Professional summary and animated stats |
| Experience | `#experience` | Three roles on a scroll-linked timeline |
| Skills | `#skills` | Capability cards, tool proficiency bars, and strength chips |
| Education | `#education` | MBA (in progress), B.Com, and a digital marketing certificate |
| Social | `#connect` | WhatsApp, LinkedIn, Instagram, Facebook, and X |
| Survey | `#survey` | Feedback form with validation |
| Contact | `#contact` | Copy buttons for email and phone, and back to top |

---

## Animations and effects

| Effect | Where | Technique |
| :--- | :--- | :--- |
| Letter flip-in | Hero name | Per-letter 3D transform with staggered delays |
| Typewriter | Hero tagline | Timed text updates |
| Scroll reveal | Sections and cards | `animation-timeline: view()` with an observer fallback |
| Timeline fill | Experience | Scroll position mapped to line height |
| Count-up | Stats | Eased `requestAnimationFrame` counter |
| Bar fill | Tool proficiency | CSS width transition on view |
| Spotlight and border glow | Glass cards | Pointer variables with a masked gradient border |
| 3D tilt | Skill cards | `perspective` and `rotateX`/`rotateY` from pointer position |
| Magnetic buttons | Buttons | Translate toward the pointer |
| Theme switch | Nav toggle | `document.startViewTransition` with a circular clip-path |
| Parallax | Background blobs | Scroll position feeds a CSS variable |
| Custom cursor | Desktop only | Eased follower with `mix-blend-mode: difference` |

---

## Browser features used

- **CSS:** custom properties, `@property`, `color-mix()`, OKLCH colours, `linear()` easing, container queries, `:has()`, `:user-invalid`, scroll-driven animations, `text-wrap: balance`
- **JavaScript:** `IntersectionObserver`, Web Animations-style timing via `requestAnimationFrame`, View Transitions API, Popover API, `<dialog>`, Clipboard API with a fallback

---

## Tech stack

Plain HTML, CSS, and vanilla JavaScript. No frameworks, no build step, and no external libraries.

---

## Getting started

**Open locally:** download `himanshu-pandey-portfolio.html` and open it in a modern browser.

**Host for free:**
- **GitHub Pages:** push the file to a repository, rename it to `index.html`, and enable Pages on the main branch.
- **Netlify or Vercel:** drag the folder into the dashboard.

---

## Customisation

Colours live in the `:root` block at the top of the stylesheet:

```css
:root{
  --a: oklch(82% .14 185);   /* accent: teal   */
  --b: oklch(66% .24 290);   /* accent: violet */
  --c: oklch(74% .2 350);    /* accent: pink   */
}
```

- **Typewriter phrases:** edit the `phrases` array in the script.
- **Reveal styles:** edit the `styles` array to change the order or add more.
- **Experience:** edit the `<article class="job">` blocks.
- **Social links:** update the `href` values in the `#connect` section.

---

## Browser support

| Browser | Support |
| :--- | :--- |
| Chrome, Edge | Full, including scroll-driven reveals and View Transitions |
| Safari 17+ | Full, with the observer fallback for some effects |
| Firefox | Core layout and animations; some newer effects fall back to simpler versions |

---

## Known limitations

- **Contact buttons copy rather than open:** email and phone buttons copy the details to the clipboard, because some preview environments block `mailto:` and `tel:` links. On your own domain, these can be changed to direct links.
- **Social links search by name:** LinkedIn, Instagram, Facebook, and X open a name search until exact profile URLs are added.
- **Survey is not stored:** responses are validated and acknowledged, but not saved. Connect it to Google Forms, Formspree, or a backend to collect answers.
- **Skill percentages are illustrative:** they are not taken from the resume.

---

## Roadmap

- [ ] Add exact profile URLs for social links
- [ ] Connect the survey to a backend or form service
- [ ] Add a downloadable PDF of the resume
- [ ] Add case studies for completed client work
- [ ] Add an optional profile photo

---

## License

All rights reserved. The content, including the name, experience, and qualifications, belongs to Himanshu Pandey. Please ask before reusing it.# Himanshu Pandey · Animated Portfolio

[![Status](https://img.shields.io/badge/status-live-22c55e?style=for-the-badge)](https://claude.ai/artifact/8i4G5gBH6QPLgGRZVHSRjf)
[![Stack](https://img.shields.io/badge/stack-HTML%20%7C%20CSS%20%7C%20JS-8b5cf6?style=for-the-badge)](#tech-stack)
[![Dependencies](https://img.shields.io/badge/dependencies-zero-5eead4?style=for-the-badge)](#tech-stack)
[![License](https://img.shields.io/badge/license-all%20rights%20reserved-f472b6?style=for-the-badge)](#license)

A single-file, animated personal website built from my resume. It presents my work as an **Accounting Executive** in Accounts Receivable, Accounts Payable, bank and credit card reconciliation, intercompany accounting, and Oracle ERP Cloud.

**Live site:** [claude.ai/artifact/8i4G5gBH6QPLgGRZVHSRjf](https://claude.ai/artifact/8i4G5gBH6QPLgGRZVHSRjf)

---

## Contents

- [Highlights](#highlights)
- [Sections](#sections)
- [Animations and effects](#animations-and-effects)
- [Browser features used](#browser-features-used)
- [Tech stack](#tech-stack)
- [Getting started](#getting-started)
- [Customisation](#customisation)
- [Browser support](#browser-support)
- [Known limitations](#known-limitations)
- [Roadmap](#roadmap)
- [License](#license)

---

## Highlights

- **Scroll-driven reveals:** sections animate in as you scroll, each with its own entrance (slide, zoom, blur-to-sharp, 3D flip, or rise).
- **Animated hero:** each letter of the name flips into place, and the tagline types out and cycles through phrases.
- **Light and dark themes:** a toggle switches themes with a circular transition that grows from the click point.
- **Glass cards:** cards with a cursor-following spotlight, a glowing gradient border, 3D tilt, and a grid that dims the others on hover.
- **Responsive layout:** works from small phones to large desktops, with container-aware skill cards.
- **Survey form:** star rating, validation, and a modal thank-you message.
- **Reduced-motion support:** animations turn off for users who prefer less motion.

---

## Sections

| Section | Anchor | Content |
| :--- | :--- | :--- |
| Hero | `#top` | Name, role, typewriter tagline, and calls to action |
| About | `#about` | Professional summary and animated stats |
| Experience | `#experience` | Three roles on a scroll-linked timeline |
| Skills | `#skills` | Capability cards, tool proficiency bars, and strength chips |
| Education | `#education` | MBA (in progress), B.Com, and a digital marketing certificate |
| Social | `#connect` | WhatsApp, LinkedIn, Instagram, Facebook, and X |
| Survey | `#survey` | Feedback form with validation |
| Contact | `#contact` | Copy buttons for email and phone, and back to top |

---

## Animations and effects

| Effect | Where | Technique |
| :--- | :--- | :--- |
| Letter flip-in | Hero name | Per-letter 3D transform with staggered delays |
| Typewriter | Hero tagline | Timed text updates |
| Scroll reveal | Sections and cards | `animation-timeline: view()` with an observer fallback |
| Timeline fill | Experience | Scroll position mapped to line height |
| Count-up | Stats | Eased `requestAnimationFrame` counter |
| Bar fill | Tool proficiency | CSS width transition on view |
| Spotlight and border glow | Glass cards | Pointer variables with a masked gradient border |
| 3D tilt | Skill cards | `perspective` and `rotateX`/`rotateY` from pointer position |
| Magnetic buttons | Buttons | Translate toward the pointer |
| Theme switch | Nav toggle | `document.startViewTransition` with a circular clip-path |
| Parallax | Background blobs | Scroll position feeds a CSS variable |
| Custom cursor | Desktop only | Eased follower with `mix-blend-mode: difference` |

---

## Browser features used

- **CSS:** custom properties, `@property`, `color-mix()`, OKLCH colours, `linear()` easing, container queries, `:has()`, `:user-invalid`, scroll-driven animations, `text-wrap: balance`
- **JavaScript:** `IntersectionObserver`, Web Animations-style timing via `requestAnimationFrame`, View Transitions API, Popover API, `<dialog>`, Clipboard API with a fallback

---

## Tech stack

Plain HTML, CSS, and vanilla JavaScript. No frameworks, no build step, and no external libraries.

---

## Getting started

**Open locally:** download `himanshu-pandey-portfolio.html` and open it in a modern browser.

**Host for free:**
- **GitHub Pages:** push the file to a repository, rename it to `index.html`, and enable Pages on the main branch.
- **Netlify or Vercel:** drag the folder into the dashboard.

---

## Customisation

Colours live in the `:root` block at the top of the stylesheet:

```css
:root{
  --a: oklch(82% .14 185);   /* accent: teal   */
  --b: oklch(66% .24 290);   /* accent: violet */
  --c: oklch(74% .2 350);    /* accent: pink   */
}
```

- **Typewriter phrases:** edit the `phrases` array in the script.
- **Reveal styles:** edit the `styles` array to change the order or add more.
- **Experience:** edit the `<article class="job">` blocks.
- **Social links:** update the `href` values in the `#connect` section.

---

## Browser support

| Browser | Support |
| :--- | :--- |
| Chrome, Edge | Full, including scroll-driven reveals and View Transitions |
| Safari 17+ | Full, with the observer fallback for some effects |
| Firefox | Core layout and animations; some newer effects fall back to simpler versions |

---

## Known limitations

- **Contact buttons copy rather than open:** email and phone buttons copy the details to the clipboard, because some preview environments block `mailto:` and `tel:` links. On your own domain, these can be changed to direct links.
- **Social links search by name:** LinkedIn, Instagram, Facebook, and X open a name search until exact profile URLs are added.
- **Survey is not stored:** responses are validated and acknowledged, but not saved. Connect it to Google Forms, Formspree, or a backend to collect answers.
- **Skill percentages are illustrative:** they are not taken from the resume.

---

## Roadmap

- [ ] Add exact profile URLs for social links
- [ ] Connect the survey to a backend or form service
- [ ] Add a downloadable PDF of the resume
- [ ] Add case studies for completed client work
- [ ] Add an optional profile photo

---

## License

All rights reserved. The content, including the name, experience, and qualifications, belongs to Himanshu Pandey. Please ask before reusing it.
