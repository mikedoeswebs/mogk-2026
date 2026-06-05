# MO Goalkeeping — mogk-2026

Website for [MO Goalkeeping](https://mogoalkeeping.co.uk) — goalkeeper coaching on the Suffolk/Essex border. Built with Astro 6, Tailwind CSS v4, and deployed on Vercel.

## Stack

- **Framework:** Astro 6 (static output)
- **Styling:** Tailwind CSS v4
- **Blog:** Astro Content Collections (Markdown)
- **Forms:** Formspree (AJAX submission)
- **Analytics:** Google Tag Manager → GA4
- **Deployment:** Vercel

## Project Structure

```
/
├── public/
│   ├── fonts/          # EdoSzn display font
│   └── images/         # Site images, banners, icons
├── src/
│   ├── components/     # Header, Footer
│   ├── content/
│   │   └── blog/       # Markdown blog posts
│   ├── layouts/        # Layout.astro, BlogLayout.astro
│   ├── pages/          # All routes
│   └── styles/
│       └── global.css  # @theme tokens, global rules
├── vercel.json
└── astro.config.mjs
```

## Commands

| Command           | Action                                      |
| :---------------- | :------------------------------------------ |
| `npm install`     | Install dependencies                        |
| `npm run dev`     | Start dev server at `localhost:4321`        |
| `npm run build`   | Build for production to `./dist/`           |
| `npm run preview` | Preview production build locally            |

## Adding a Blog Post

Create a new `.md` file in `src/content/blog/` with this frontmatter:

```markdown
---
title: Your Post Title
date: 2026-01-01
excerpt: A short summary shown in listings.
category: Coaching
---

Post content here...
```

The slug is derived from the filename. The post will appear automatically on `/blog/`.
