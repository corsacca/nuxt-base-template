# Nuxt Base Template

A starter template for apps built on [nuxt-base](https://github.com/corsacca/nuxt-base).

## Quick Start

### 1. Clone this template

```bash
npx giget gh:corsacca/nuxt-base-template my-app
cd my-app
```

### 2. Configure environment

```bash
cp .env.example .env
```

Edit `.env` with your values:
- `DATABASE_URL` - PostgreSQL connection string (required)
- `JWT_SECRET` - A secure random string (required)
- `APP_TITLE` - Your app name

**Important:** Do NOT wrap values in quotes.

### 3. Install and run

```bash
npm install
npm run dev
```

Migrations run automatically. Your app is ready at http://localhost:3000

## What's Included

This template provides:

- **Pages**: Landing, login, register, dashboard, profile, password reset
- **Layouts**: Default (authenticated) and auth (centered cards)
- **Configured**: nuxt.config.ts with base layer, package.json with dependencies

The [nuxt-base](https://github.com/corsacca/nuxt-base) layer provides:

- Authentication (JWT, email verification, password reset)
- Theme system (light/dark mode)
- Email (SMTP templates)
- S3 storage
- Database utilities (PostgreSQL)
- API routes

## Customization

All files in this template are yours to modify:

- Edit pages in `app/pages/`
- Customize layouts in `app/layouts/`
- Add components in `app/components/`
- Extend `nuxt.config.ts` as needed

## Documentation

Copy `BASE_LAYER.md` from the layer for API reference:

```bash
cp node_modules/.c12/github_corsacca_nuxt_*/BASE_LAYER.md .
```

See the [nuxt-base repository](https://github.com/corsacca/nuxt-base) for full documentation.
