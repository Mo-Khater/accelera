# Benchmark Platform

The Benchmark Platform is a web application for managing datasets, metrics,
submissions, users, dashboards, and leaderboards. It is implemented as a Node.js
backend plus a Vite React frontend under `benchmark/`.

## Overview

The platform supports the workflow around evaluating ML pipelines: define a
benchmark, define metrics, submit results, and compare submissions through a
leaderboard-oriented UI.

## Source Layout

```text
benchmark/
  backend/
    server.js
    routes/
    schemas/
    validations/
    middleware/
    scripts/
  frontend/
    src/
      components/
      App.jsx
      main.jsx
```

## Backend

The backend is an Express application with route modules for:

- Benchmarks
- Metrics
- Submissions
- Users

It includes schemas, validation logic, authentication middleware, admin
middleware, and scoring utility scripts.

## Frontend

The frontend is a Vite React app with screens and components for:

- Home
- Login and signup
- Dashboard and admin dashboard
- Benchmarks
- Metrics
- Submission display
- Leaderboard

## Run Locally

This project requires Node.js `v22.23.0`.

```bash
cd benchmark/backend
npm install
npm run dev
```

In another terminal:

```bash
cd benchmark/frontend
npm install
npm run dev
```

## Related Modules

- [AutoML](automl.md) - Generate and evaluate candidate model pipelines.
- [Core Pipeline](core-pipeline.md) - Build graph pipelines for experiments.
- [Deployment](deployment.md) - Serve selected model artifacts.
