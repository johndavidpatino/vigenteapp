# Vigente App / Senior Connexion - Agent Instructions

## Product intent
Vigente App explores the Senior Connexion concept: a warm, human-centered companion app for Colombian adults around 60 to 74 years old.

The interface must feel:
- warm, calm, trustworthy and premium
- human, never robotic
- easy to read and easy to touch
- emotionally supportive, not clinical

## Visual identity
Use the design system in `src/styles/`.

Do not invent new colors unless explicitly requested.

Primary tokens:
- teal: `#007D7A`
- teal dark: `#005F63`
- navy: `#0B3558`
- coral: `#F26B55`
- cream: `#FFF9EF`
- mint: `#EAF7F4`
- soft blue: `#EEF7FF`
- peach: `#FFF1E6`
- lavender: `#F3EEFF`

## Accessibility rules
- Minimum touch target: 56px.
- Use large typography.
- Avoid dense screens.
- Use clear Spanish labels.
- Prefer cards, friendly icons, short copy and direct actions.
- Add meaningful `aria-label` attributes when needed.

## Implementation rules
- Reuse CSS classes from `src/styles/components.css`.
- Do not use inline styles.
- Do not duplicate design tokens.
- Keep mobile-first layout.
- Keep changes small and focused.
- Do not rewrite unrelated files.

## Current prototype
This repo currently contains a static HTML/CSS prototype only. It is intentionally framework-agnostic so it can later be translated to React Native, Expo, native Swift/Kotlin, Razor, or a web app.
