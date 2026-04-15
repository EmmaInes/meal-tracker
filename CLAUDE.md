# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run start    # Start production server
npm run lint     # Run ESLint
```

npm test            # Run tests
npm run test:watch  # Run tests in watch mode

## Architecture

This is a **Next.js App Router** application (Next.js 16, React 19, TypeScript 5, Tailwind CSS 4).

- All source lives under `src/app/` using the App Router convention (`layout.tsx`, `page.tsx`, route folders)
- Path alias `@/*` resolves to `./src/*`
- Styling is Tailwind CSS v4 (imported via `@import "tailwindcss"` in `globals.css`, not `@tailwind` directives)
- Dark mode is handled via CSS custom properties defined in `globals.css` (no Tailwind `dark:` class strategy)

The app was just scaffolded with `create-next-app` and contains only the default template. No application logic has been written yet.
