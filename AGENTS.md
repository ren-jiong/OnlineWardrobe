# Project Rules for Online Wardrobe App

## Role
You are assisting a beginner developer to build and maintain a Flutter-based wardrobe app. Prioritize simplicity, readability, and maintainability.

## Tech Stack
- Use Flutter and Dart.
- Do not switch to React Native, Swift, Kotlin, Vue, or other frameworks.
- Use local-first storage. No backend server unless explicitly requested.
- Store clothing images locally on device.
- Use a local database for metadata.
- Use external APIs only for weather and LLM-based outfit recommendation.

## Architecture
Use the following folders:
- lib/pages: screens
- lib/widgets: reusable UI components
- lib/models: data models
- lib/services: weather, LLM, image segmentation, local file services
- lib/repositories: database access
- lib/utils: helper functions

## Dependency Rules
- Do not add new production dependencies without explaining why.
- Before adding a dependency, check whether existing dependencies can solve the problem.
- Avoid mixing multiple state management systems.
- Prefer simple implementation over over-engineered architecture.

## Coding Rules
- Before editing code, explain:
  1. which files will be changed;
  2. why they need to be changed;
  3. whether new dependencies are required;
  4. how to test the change.
- Make small changes per task.
- Do not refactor unrelated files.
- Keep UI and business logic separated.
- Add comments for non-obvious logic.

## Product Scope
Current MVP features:
1. Add clothing by photo.
2. Save clothing image locally.
3. Save clothing metadata locally.
4. Display wardrobe board by category.
5. Mark clothing as washed/unwashed.
6. Filter unsuitable clothing based on weather.
7. Generate outfit recommendations using LLM API.
8. Basic outfit preview.

Do not implement:
- User accounts.
- Cloud sync.
- Social sharing.
- E-commerce.
- Community features.
- Complex recommendation engine.
- Multi-user system.
unless explicitly requested.