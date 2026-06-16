# Language & Culture Organisation Astro Template

This is a visual Astro template for an organisation website focused on learning a language and culture.

The template includes:

- Logo placeholder using the word `logo`
- Header with two generic language buttons: `Language 1` and `Language 2`
- Homepage posts/news cards
- Interactive event calendar
- A design-selection page for customers
- 20 visual design paths that reuse the same content
- A clear central switcher on every design preview page
- Interaction pattern notes that can be combined with any design

## Run locally

```bash
npm install
npm run dev
```

## Main paths

```text
/                         Main template
/designs                  Design gallery for customer choice
/designs/glassmorphism
/designs/neumorphism
/designs/skeuomorphism
/designs/flat-design
/designs/material-design
/designs/minimalism
/designs/maximalism
/designs/brutalism
/designs/anti-design
/designs/claymorphism
/designs/bento-grid
/designs/gradient-design
/designs/dark-mode
/designs/aurora-glow
/designs/retro-y2k
/designs/cyberpunk-futuristic
/designs/editorial-design
/designs/corporate-clean
/designs/organic-natural
/designs/swiss-typographic
```

## Main files

```text
src/pages/index.astro
src/pages/designs/index.astro
src/pages/designs/[slug].astro
src/components/Header.astro
src/components/Calendar.astro
src/components/PostCard.astro
src/components/DesignSwitcher.astro
src/data/posts.ts
src/data/events.ts
src/data/designOptions.ts
src/styles.css
```

## How it works

All design preview pages use the same content from `src/data/posts.ts` and `src/data/events.ts`.

The design paths are generated from `src/data/designOptions.ts` by `src/pages/designs/[slug].astro`.

Every design page includes `src/components/DesignSwitcher.astro`, which creates a clear middle-page button and dropdown for switching design previews.
