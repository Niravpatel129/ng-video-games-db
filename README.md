# Angular Video Games DB

An Angular 11 video game discovery app that lists games, supports search routes, and opens detail pages for individual games.

The app uses a shared HTTP service to load game lists, game details, screenshots, and trailers from an API configured through the Angular environment files.

## Features

- Home page with game listing
- Search route for filtering games by query
- Game detail route by ID
- Shared HTTP service for API calls
- Combined detail, screenshot, and trailer requests with RxJS `forkJoin`
- Angular Material/CDK dependencies available for UI work
- Gauge dependency available for rating or score visualization

## Tech stack

- Angular 11
- TypeScript
- Angular Router
- Angular Material / CDK
- RxJS
- Angular Gauge
- Karma / Jasmine
- Protractor

## Getting started

Install dependencies:

```bash
npm install
```

Run the local development server:

```bash
npm start
```

Open the app locally:

```text
http://localhost:4200
```

## Available scripts

```bash
npm start       # Run Angular dev server
npm run build   # Build the app
npm test        # Run unit tests
npm run lint    # Run linting
npm run e2e     # Run end-to-end tests
```

## Routes

```text
/                    # Home game listing
/search/:game-search # Search-filtered game listing
/details/:id         # Game detail page
```

## Project structure

```text
src/app/components/      # Home, details, search, and UI components
src/app/services/        # API service layer
src/app/models/          # API response and game models
src/environments/        # API base URL and environment config
```

## Configuration

The API base URL is read from the Angular environment config:

```ts
environment.BASE_URL
```

Make sure the environment file points to the correct games API before running or deploying the app.

## Status

This is a learning/demo Angular project for game discovery UI patterns, routing, and API integration.
