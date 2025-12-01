# FlowOncology Web Application

FlowOncology WebApp is a Next.js application scaffolded with the App Router, React, TypeScript, and Tailwind CSS. It provides a clean foundation for building oncology-focused features and workflows.
This project is in progress and does not yet encompass the complete architecture of the FlowOncology platform.

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
src/
├── app/
│   ├── layout.tsx                 # Root layout
│   ├── page.tsx                   # Main entry point (uses FlowOncologyApp)
│   └── globals.css                # Global styles
│
├── components/
│   ├── layout/
│   │   ├── Sidebar.tsx           # Sidebar navigation component
│   │   └── Header.tsx            # Top header with search
│   │
│   ├── dashboard/
│   │   ├── DashboardView.tsx     # Main dashboard container
│   │   ├── RecentPatients.tsx    # Recent patients list
│   │   ├── PatientCard.tsx       # Individual patient card
│   │   └── StudiesGrid.tsx       # New studies section
│   │
│   ├── patient/
│   │   ├── PatientDetailView.tsx      # Patient detail container
│   │   ├── PatientHeader.tsx          # Patient info header
│   │   ├── PatientTabs.tsx            # Tab navigation
│   │   ├── TestHistoryTimeline.tsx    # Test history timeline view
│   │   ├── TestDetailsView.tsx        # Detailed test view
│   │   ├── TreatmentHistoryTimeline.tsx  # Treatment timeline
│   │   └── TreatmentDetailsView.tsx   # Detailed treatment view
│   │
│   └── ui/
│       ├── Button.tsx            # Reusable button component
│       ├── Card.tsx              # Reusable card component
│       ├── Badge.tsx             # Status badges
│       └── Input.tsx             # Form inputs
│
├── types/
│   ├── index.ts                  # Export all types
│   ├── patient.ts                # Patient related types
│   ├── test.ts                   # Test related types
│   ├── treatment.ts              # Treatment related types
│   └── study.ts                  # Study related types
│
├── data/
│   ├── mockPatients.ts           # Mock patient data
│   ├── mockStudies.ts            # Mock studies data
│   ├── mockTests.ts              # Mock test data
│   └── mockTreatments.ts         # Mock treatment data
│
├── hooks/
│   ├── usePatientData.ts         # Custom hook for patient operations
│   ├── useSearch.ts              # Search functionality hook
│   └── useNavigation.ts          # Navigation state management
│
├── lib/
│   ├── utils.ts                  # Utility functions
│   └── constants.ts              # App constants
│
└── styles/
    └── tailwind.config.js        # Tailwind configuration
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
