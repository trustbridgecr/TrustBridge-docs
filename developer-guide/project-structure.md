# Project Structure

This document provides an overview of the folder and file organization within the TrustBridge dApp repository.

## Root Directory

- `.env.example`: Sample environment variables file.
- `.eslintrc.json`: ESLint configuration.
- `.gitignore`: Specifies files and directories to be ignored by Git.
- `.lintstagedrc`: Configuration for lint-staged.
- `.prettierrc`: Prettier configuration.
- `CONTRIBUTING.md`: Guidelines for contributing to the project.
- `README.md`: Project overview and setup instructions.
- `components.json`: Component configuration file.
- `eslint.config.mjs`: ESLint module configuration.
- `firebase.ts`: Firebase initialization script.
- `next.config.ts`: Next.js configuration.
- `package.json`: Project dependencies and scripts.
- `postcss.config.mjs`: PostCSS configuration.
- `tsconfig.json`: TypeScript configuration.

## Folders

### `.github/`

Contains GitHub-specific configurations, such as workflows and issue templates.

### `.husky/`

Husky hooks for managing Git hooks, ensuring code quality before commits.

### `docs/`

Documentation files for the project.

### `public/`

Static assets like images and icons accessible publicly.

### `src/`

Main source code directory.

#### `src/components/`

Reusable React components used throughout the application.

#### `src/pages/`

Next.js pages corresponding to different routes in the application.

#### `src/styles/`

Global and component-specific stylesheets.

#### `src/utils/`

Utility functions and helpers.

#### `src/hooks/`

Custom React hooks for managing state and side effects.

#### `src/context/`

React context providers for global state management.

#### `src/services/`

Modules for interacting with external APIs and services.

#### `src/config/`

Configuration files and constants used across the application.

---

Next: [API & Hooks](api.md)
