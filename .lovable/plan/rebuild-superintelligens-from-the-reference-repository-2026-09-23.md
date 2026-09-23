# Rebuild SUPERINTELLIGENS from the reference repository

## Scope
- Replace the placeholder with the SUPERINTELLIGENS landing experience at `/`.
- Add the matching `/login` and `/workspace` screens.
- Add the `/api/chat` and `/api/generate` request handlers, preserving the reference app’s local fallback behavior.
- Bring over the reference components, styling, fonts, images, icons, and installable-app assets.
- Preserve TanStack Start, React 19, Tailwind 4, and the project’s existing error handling.

## Implementation
- Copy the public repository’s application source and static assets into this project, excluding Git metadata and generated build output.
- Align dependencies with the reference repository.
- Keep API keys server-side; without a Gemini key, the workspace will still use the reference app’s built-in deterministic generation/chat fallbacks.
- Verify `/`, `/login`, and `/workspace` on desktop and mobile, then exercise one workspace generation flow and both API endpoints.
