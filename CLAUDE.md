# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

- `yarn dev`: Run development server
- `yarn build`: Build for production
- `yarn start`: Start production server
- `yarn lint`: Run ESLint to check code
- `yarn test`: Run Jest tests
- `yarn test:watch`: Run tests in watch mode
- `yarn test -- -t "test name"`: Run a specific test

## Code Style

- **Formatting**: Use Prettier with semicolons, single quotes, 2 space indentation, 80 character line limit
- **Imports**: Group imports by type (React, external libs, internal components, types/interfaces)
- **Components**: Use named function exports and functional components with TypeScript
- **Naming**: Use kebab-case for files, PascalCase for components/interfaces, camelCase for variables/functions
- **Error Handling**: Use try/catch blocks with proper error logging and typed error classes
- **Types**: Prefer typed props and return types, use interface for public APIs, avoid `any`

## Architecture

- Next.js app router with API routes in `/app/api`
- Component structure follows `/components/{feature}/{component-name}.tsx` pattern
- Use SWR for data fetching with typed hooks
- State management via Context where appropriate
