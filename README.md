# HTML5-Semantic-Structure-Accessibility
# Semantic & Accessible Portfolio Webpage


To access the webpage click the below link:
 https://neerajjkm.github.io/HTML5-Semantic-Structure-Accessibility/

A production-ready, fully semantic skeleton for a modern portfolio website engineered specifically to achieve **100/100 Lighthouse Accessibility** and **100/100 Lighthouse SEO** scores.

The document structure and semantic architecture directly adhere to the principles outlined in Dave Gray's tutorial [*Semantic HTML Tags | HTML5 Semantic Elements Tutorial*](https://www.youtube.com/watch?v=kX3TfdUqpuU).

---

## 🌟 Key Features

- **Strict Document Hierarchy:** Exactly one `<h1>` per page serving as the primary outline anchor, followed predictably by `<h2>` for distinct topics/articles and `<h3>` for nested subtopics—guaranteeing clean document outlines.
- **Full Landmark Architecture:** Built with dedicated HTML5 landmarks (`<header>`, `<main>`, `<section>`, `<article>`, `<aside>`, and `<footer>`) to enable seamless assistive navigation via screen readers.
- **Disambiguated Landmarks:** Differentiates multiple `<nav>` landmarks using unique `aria-label` tags (`Primary navigation` vs. `Footer links`).
- **Zero Div Soup:** Leverages specialized elements such as `<article>` for self-contained entities, `<figure>` and `<figcaption>` for media semantics, and `<time datetime="...">` for machine-readable dates and durations.
- **Lighthouse 100 SEO Ready:** Built-in canonical link, meta description, robots directives, Open Graph cards, responsive meta viewport, and proper language declaration (`<html lang="en">`).
- **WCAG 2.2 AA Keyboard Accessibility:** Includes an accessible skip-link (`#main-content`) and programmatic form label associations (`for`/`id`).

---

## 📁 Repository Structure

```text
├── index.html        # Fully semantic & accessible portfolio skeleton
└── README.md         # Documentation and audit verification guidelines
```

---

## 🧱 Landmark & Semantic Hierarchy

Based on Dave Gray's semantic guidelines:

```text
<body>
  ├── a.skip-link (Keyboard bypass mechanism)
  ├── <header>
  │     ├── <h1> (Alex Rivera)
  │     └── <nav aria-label="Primary navigation">
  ├── <main id="main-content">
  │     ├── <section id="about">
  │     │     ├── <h2> (About Me)
  │     │     └── <aside aria-label="Core proficiencies">
  │     │           └── <h3> (Core Competencies)
  │     ├── <section id="projects">
  │     │     ├── <h2> (Featured Projects)
  │     │     ├── <article> (Project 1)
  │     │     └── <article> (Project 2)
  │     ├── <section id="experience">
  │     │     ├── <h2> (Work History)
  │     │     └── <article>
  │     └── <section id="contact">
  │           ├── <h2> (Get in Touch)
  │           └── <form> (Accessible inputs & labels)
  └── <footer>
        ├── <nav aria-label="Footer links">
        └── <p> (&copy; <time>)
```

---

## 🧪 Lighthouse Audit Checklist

| Audit Category | Criteria Met | Standard Followed |
| :--- | :--- | :--- |
| **Accessibility** | Complete semantic landmark tree | WCAG 2.2 & HTML5 Spec |
| **Accessibility** | Strict linear heading order (`h1` &rarr; `h2` &rarr; `h3`) | No skipped heading tiers |
| **Accessibility** | Distinct navigation labelling (`aria-label`) | Accessible naming for multiple `<nav>` tags |
| **Accessibility** | Fully associated form labels | `label[for]` matches `input[id]` |
| **Accessibility** | Direct content bypass mechanism | `.skip-link` pointing to `#main-content` |
| **SEO** | Crawlability & Indexing metadata | Canonical, Robots, Description tags |
| **SEO** | Mobile-ready viewport | `width=device-width, initial-scale=1.0` |
| **SEO & Performance**| Explicit image dimensions & `loading="lazy"` | Zero Cumulative Layout Shift (CLS) |

---
