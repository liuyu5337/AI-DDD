# Project Rules

## Project overview
- This is an enterprise application with backend, frontend, and docs modules.
- Backend uses Spring Boot 3.x, frontend uses Vue 3 + Element Plus.
- Prefer small, reversible changes.

## Engineering rules
- Do not rename modules or move directories unless explicitly required.
- Do not introduce new frameworks without justification.
- Keep API contracts backward compatible unless task says otherwise.
- Write or update tests when changing behavior.
- Update docs when changing public APIs, configs, or scripts.

## Code style
- Backend: prefer clear service boundaries, DTO/VO separation, no giant methods.
- Frontend: keep API calls centralized, avoid business logic inside components when possible.
- Config: never hardcode secrets, tokens, or passwords.

## Delivery format
- Always report:
  1. what changed
  2. affected files
  3. risks
  4. follow-up suggestions