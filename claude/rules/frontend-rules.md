# Frontend Rules

## Baseline
- Vue 3
- Composition API
- Element Plus

## Structure
- views focus on composition and interaction flow
- reusable components for repeated patterns
- composables for reusable state / behavior
- API calls must be centralized

## UX rules
- loading / empty / error / no-permission states must be explicit
- destructive actions require confirmation
- form validation messages must be clear and consistent
- table column names, placeholders, and buttons should use stable wording

## Integration
- do not silently invent backend behavior
- keep route / page / permission assumptions explicit
- distinguish display model from raw API model when needed

## Maintainability
- avoid heavy business logic in templates
- avoid unrelated UI refactors in delivery tasks
