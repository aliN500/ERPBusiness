# ERPBusiness

ERP business application built with [Next.js](https://nextjs.org).

## Tech Stack

- **Framework**: Next.js 16 (App Router, Turbopack)
- **Language**: TypeScript (strict mode)
- **Styling**: Tailwind CSS v4
- **Linting**: ESLint 10 (flat config, `eslint-config-next`)
- **Formatting**: Prettier

## Prerequisites

- Node.js 20.9 or later (LTS recommended)
- A package manager: npm, pnpm, or yarn

## Getting Started

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Scripts

- `npm run dev` — start the dev server (Turbopack)
- `npm run build` — create a production build
- `npm run start` — serve the production build
- `npm run lint` — lint the codebase with ESLint
- `npm run typecheck` — type-check with `tsc --noEmit`
- `npm run format` — format the codebase with Prettier

## Project Structure

```
app/
  layout.tsx   # Root layout (metadata, fonts)
  page.tsx     # Home page
  globals.css  # Global styles + Tailwind theme
public/        # Static assets (add as needed)
components/    # Reusable UI components (add as needed)
lib/           # Shared utilities (add as needed)
```

## Environment Variables

Copy `.env.example` to `.env.local` and fill in your values:

```bash
cp .env.example .env.local
```

Only variables prefixed with `NEXT_PUBLIC_` are exposed to the browser.
