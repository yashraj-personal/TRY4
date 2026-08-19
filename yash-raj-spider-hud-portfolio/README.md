# Yash Raj — Spider-HUD Portfolio

A cinematic, static-friendly portfolio experience for Yash Raj: cybersecurity enthusiast, AI/ML learner and web builder.

## Features

- Skippable system boot sequence with responsive HUD hero
- Mission dossiers, capability network, achievements and education timeline
- Spider-Sense mode, CTRL+K terminal, interactive hanging-avatar-ready visual language
- Local WEB AI assistant using only the portfolio facts (no API key)
- Web Audio interface tones, explicitly OFF by default
- Phone/email secure channel with no pretend submission
- Source ZIP download from the footer

## Run locally

```bash
cd frontend
yarn install
yarn start
```

The frontend uses `REACT_APP_BACKEND_URL` for the source ZIP endpoint. The FastAPI service runs on the configured supervisor port and does not need to be started manually.

## Editing portfolio content

Project and skill content lives at the top of `frontend/src/App.js` in the `projects`, `skills`, and navigation arrays. Replace the supplied image URLs there if you want to use local assets. GitHub and LinkedIn intentionally remain `ADD YOUR LINK` placeholders until real URLs are available.

## GitHub Pages

1. Create a repository and upload the project files.
2. If deploying the React build, run `yarn build` inside `frontend`.
3. Publish the generated `frontend/build` directory using your preferred Pages workflow.
4. Keep the supplied asset URLs or move the images into `frontend/public/assets` and update the constants.
5. If hosting as fully static-only, the core portfolio works without the API; only the source ZIP button needs a static download file.

## Accessibility and performance

The interface uses semantic sections, keyboard-accessible controls, visible focus states, reduced-motion CSS, lazy loading for below-fold images, and a CSS/SVG atmosphere rather than a heavy 3D runtime. Sound never starts without an explicit toggle.
