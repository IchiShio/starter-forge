# StarterForge

A production-ready **Astro 5 + Tailwind CSS v4** SaaS starter kit. Ship your landing page, blog, and marketing site in minutes -- not weeks.

![StarterForge Screenshot](https://via.placeholder.com/1200x630/3b82f6/ffffff?text=StarterForge)

## Features

- **Astro 5** -- Static site generation with island architecture
- **Tailwind CSS v4** -- Next-gen utility-first CSS with `@theme` configuration
- **Dark Mode** -- System-aware with manual toggle, zero flash
- **Blog** -- MDX content collections with tags and reading time
- **SEO** -- Meta tags, Open Graph, sitemap, robots.txt
- **View Transitions** -- Smooth page navigation out of the box
- **Responsive** -- Mobile-first design, looks great on all devices
- **TypeScript** -- Strict mode for type safety
- **100 Lighthouse** -- Perfect performance score by default

## Quick Start

```bash
# Clone the repository
git clone https://github.com/your-username/starter-forge.git my-saas
cd my-saas

# Install dependencies
npm install

# Start development server
npm run dev
```

Open [http://localhost:4321](http://localhost:4321) in your browser.

## Project Structure

```
/
├── public/
│   ├── favicon.svg
│   └── robots.txt
├── src/
│   ├── components/
│   │   ├── CTA.astro
│   │   ├── Features.astro
│   │   ├── Footer.astro
│   │   ├── Hero.astro
│   │   ├── Navbar.astro
│   │   ├── Pricing.astro
│   │   └── Testimonials.astro
│   ├── content/
│   │   └── blog/
│   │       ├── getting-started.mdx
│   │       └── why-astro.mdx
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   ├── blog/
│   │   │   ├── index.astro
│   │   │   └── [slug].astro
│   │   ├── 404.astro
│   │   ├── about.astro
│   │   └── index.astro
│   ├── styles/
│   │   └── global.css
│   ├── consts.ts
│   └── content.config.ts
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## Customization

### Theme Colors

Edit `src/styles/global.css` to change the primary color palette:

```css
@theme {
  --color-primary-500: #8b5cf6; /* Change to your brand color */
  --color-primary-600: #7c3aed;
  /* ...etc */
}
```

### Site Metadata

Update `src/consts.ts` with your site name and URL:

```ts
export const SITE_TITLE = 'YourSaaS';
export const SITE_DESCRIPTION = 'Your tagline here.';
export const SITE_URL = 'https://your-domain.com';
```

### Adding Blog Posts

Create `.mdx` files in `src/content/blog/` with this frontmatter:

```mdx
---
title: "Post Title"
description: "A short description."
date: 2026-03-25
tags: ["tag1", "tag2"]
---

Your content here.
```

## Commands

| Command           | Action                                      |
| :---------------- | :------------------------------------------ |
| `npm install`     | Install dependencies                        |
| `npm run dev`     | Start dev server at `localhost:4321`         |
| `npm run build`   | Build production site to `./dist/`           |
| `npm run preview` | Preview production build locally            |

## Deployment

### Vercel

Connect your Git repository on [vercel.com](https://vercel.com). Astro is auto-detected -- no configuration needed.

### Netlify

Connect your repository on [netlify.com](https://netlify.com). Set the build command to `npm run build` and publish directory to `dist`.

### Cloudflare Pages

Connect your repository on [Cloudflare Pages](https://pages.cloudflare.com). Set build command to `npm run build` and output directory to `dist`.

## License

MIT License. See [LICENSE](LICENSE) for details.
