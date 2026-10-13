# Acme Dashboard

A Next.js dashboard application for managing customers, invoices, and revenue insights. This project is built with the Next.js App Router and uses a PostgreSQL-backed data layer to power the dashboard UI.

## Overview

This application includes:
- A landing page and login flow
- A dashboard overview with summary cards
- Revenue reporting and recent invoice activity
- Invoice and customer management screens
- Search and pagination for invoice data
- Tailwind-based styling with a responsive layout

## Tech Stack

- Next.js
- React
- TypeScript
- Tailwind CSS
- PostgreSQL
- NextAuth
- Heroicons

## Project Structure

- `app/` - application routes and pages
- `app/ui/` - reusable UI components and dashboard views
- `app/lib/` - data fetching and database logic
- `public/` - static assets
- `tailwind.config.ts` - Tailwind configuration
- `next.config.ts` - Next.js configuration

## Prerequisites

Before running the project, make sure you have:
- Node.js 18+ installed
- pnpm installed
- A PostgreSQL database connection available for `POSTGRES_URL`

## Getting Started

1. Install dependencies:

```bash
pnpm install
```

2. Create your environment file:

```bash
cp .env.example .env.local
```

3. Add your database and auth values to `.env.local`:

```env
POSTGRES_URL=
POSTGRES_PRISMA_URL=
POSTGRES_URL_NON_POOLING=
POSTGRES_USER=
POSTGRES_HOST=
POSTGRES_PASSWORD=
POSTGRES_DATABASE=
AUTH_SECRET=
AUTH_URL=http://localhost:3000/api/auth
```

4. Start the development server:

```bash
pnpm dev
```

Then open http://localhost:3000 in your browser.

## Available Scripts

```bash
pnpm dev
pnpm build
pnpm start
```

## Notes

This project is configured as a starter dashboard app and is intended to demonstrate modern Next.js patterns, data fetching with Server Components, and a responsive admin UI.

