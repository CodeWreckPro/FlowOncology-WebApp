# FlowOncology Web Application

FlowOncology WebApp is a Next.js application scaffolded with the App Router, React, TypeScript, and Tailwind CSS. It provides a clean foundation for building oncology-focused features and workflows.

## Overview
- Built on `Next.js 15` with the App Router (`src/app`)
- Uses `React 19` and `TypeScript 5`
- Styling with `Tailwind CSS v4` via `@tailwindcss/postcss`
- Minimal, production-ready structure with static assets under `public/`

## Tech Stack
- Framework: `next@15.5.6`
- UI: `react@19.1.0`, `react-dom@19.1.0`
- Language: `typescript@^5`
- Styles: `tailwindcss@^4`, `@tailwindcss/postcss@^4`

## Quick Start
1. Install dependencies: `npm install`
2. Run in development: `npm run dev`
3. Build for production: `npm run build`
4. Start production server: `npm start`

## Scripts
- `npm run dev` — starts the Next.js dev server with Turbopack
- `npm run build` — builds the app with Turbopack
- `npm start` — runs the production server

## Project Structure
```
FlowOncology-WebApp/
├── public/                     # Static assets available at the site root
│   ├── next.svg
│   ├── vercel.svg
│   ├── file.svg
│   ├── globe.svg
│   └── window.svg
│
├── src/
│   └── app/
│       ├── favicon.ico         # Application favicon
│       ├── globals.css         # Global styles (imports Tailwind)
│       ├── layout.tsx          # Root layout and metadata
│       └── page.tsx            # Home page
│
├── next.config.ts              # Next.js configuration
├── postcss.config.mjs          # Tailwind/PostCSS plugin config
├── tsconfig.json               # TypeScript configuration
├── package.json                # Dependencies and scripts
├── package-lock.json           # NPM lockfile
└── .gitignore                  # Git ignore patterns
```

## Configuration Notes
- Tailwind is enabled by importing `@import "tailwindcss";` in `src/app/globals.css`
- Fonts are loaded using `next/font` and wired into CSS variables for Tailwind usage
- TypeScript is set to `strict` with `noEmit` and `isolatedModules`

## Public Folder
The `public/` directory contains static files served from the site root. Files here are accessible at paths like `/next.svg` and can be used by components such as `next/image`. Use this folder for icons, images, and any asset that should be directly accessible without bundling.

## Deployment
- Build with `npm run build`
- Serve with `npm start` or deploy to platforms like Vercel

## License
This project is licensed under the MIT License. See `LICENSE` for details.
