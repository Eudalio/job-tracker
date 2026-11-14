# Job Tracker

Web app for browsing job postings and tracking your applications. Three main areas are planned: **Jobs**, **Applications**, and **Dashboard**.

## Stack

- Angular 22 (standalone components, routing)
- SCSS
- ESLint (`angular-eslint`) + Prettier

## Prerequisites

- Node.js 20+
- npm 10+

## Setup

```bash
npm install
```

## Development

```bash
npm start
```

Open [http://localhost:4200/](http://localhost:4200/). The app reloads on file changes.

## Scripts

| Command                | Description                           |
| ---------------------- | ------------------------------------- |
| `npm start`            | Dev server (`ng serve`)               |
| `npm run build`        | Production build                      |
| `npm test`             | Unit tests (Vitest)                   |
| `npm run lint`         | ESLint on `src/**/*.ts` and templates |
| `npm run format`       | Format with Prettier                  |
| `npm run format:check` | Check formatting without writing      |

## Project structure

```
src/app/
  core/          # Singleton services, interceptors, app-wide providers
  shared/        # Reusable UI and utilities
  features/
    jobs/        # Job listings (Arbeitnow, filters, table)
    applications/ # Track applications (forms, CRUD)
    dashboard/   # Overview by pipeline stage
```

Feature screens and layout land in later issues; this repo only establishes the folder layout.

## Additional resources

- [Angular CLI](https://angular.dev/tools/cli)
