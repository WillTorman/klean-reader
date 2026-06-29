# Klean Reader Mobile

Mobile app for Klean Reader, planned with React Native.

## Status

This folder is currently a placeholder.
Web is being built first.
Mobile implementation will start after the web app reaches a stable milestone.

## Goals

- Build one app that runs on Android and iOS
- Reuse as much domain logic as possible from the web app
- Keep platform-specific code isolated and minimal

## Planned Stack

- React Native
- Expo (recommended default for faster setup and iteration)
- TypeScript
- React Navigation
- API and business logic shared from root-level packages when available

## Planned Folder Structure

mobile/
  src/
    app/
    features/
    components/
    screens/
    navigation/
    services/
    hooks/
    utils/
    types/
  assets/
    images/
    fonts/
  app.json
  package.json
  tsconfig.json
  README.md

If using Expo prebuild or bare React Native, native folders may also appear:

- android/
- ios/

## Development Plan

1. Initialize app with Expo and TypeScript
2. Set up navigation and base screen layout
3. Add auth flow and API client
4. Build core reader views
5. Introduce shared logic from monorepo packages
6. Add offline/cache support
7. Prepare store-ready builds for Android and iOS

## Setup Notes For Later

Recommended initialization command:

npx create-expo-app@latest . --template

Then choose:
- Blank (TypeScript)

After setup, expected common scripts in package.json:

- start
- android
- ios
- web
- lint
- test

## Architecture Notes

- Keep business logic framework-agnostic when possible
- Keep UI components platform-aware only when necessary
- Prefer feature-based organization over type-based sprawl

## Quality Checklist

- TypeScript checks passing
- Lint passing
- Basic smoke tests for navigation and key screens
- API error handling and empty states
- Responsive layouts for common phone sizes

## Next Milestone

Initialize Expo app and commit the first runnable mobile baseline.
