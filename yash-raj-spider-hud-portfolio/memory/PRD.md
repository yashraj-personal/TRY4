# Yash Raj Spider-HUD Portfolio

## Original problem statement
Build a complete cinematic, premium Spider-HUD-inspired portfolio website for Yash Raj, a Class 12 PCM + Computer Science student and cybersecurity enthusiast. It must present accurate AI/ML, cybersecurity, Python, Linux and web projects with an interactive operating-system feel, skippable boot sequence, responsive HUD, local portfolio assistant, source ZIP download, and no fabricated links or claims.

## Architecture decisions
- React frontend remains the primary experience for the provided app shell; core content is static-friendly and uses the configured asset URLs.
- FastAPI adds a source-packaging endpoint at `/api/download-source`; it excludes environment files, dependencies, caches and generated archives.
- Portfolio content is data-driven near the top of `frontend/src/App.js` for beginner-friendly editing.
- WEB AI is local/predefined and Web Audio is generated only after explicit opt-in; no external AI key is exposed.

## Implemented
- Cinematic boot screen with sequential-style system copy, Enter System and Skip Intro.
- Framed Spider man 1 hero, asymmetric editorial typography, responsive HUD header and Spider-Sense toggle.
- Identity, Mission Database dossiers, Arsenal skill network, achievements, mission log and Secure Channel contact display.
- Local WEB AI panel, CTRL+K terminal easter egg, generated sound toggle, source ZIP download and mobile/reduced-motion behavior.
- Metadata, custom circular Y web-mark favicon, 1200×630 SVG social preview card, README setup/deployment notes, data-testid coverage, and tested desktop/mobile flows.

## Prioritized backlog
- P0: None; current tested experience is functional.
- P1: Replace the supplied remote image URLs with repository-local optimized assets for fully self-contained GitHub Pages exports.
- P1: Add real GitHub and LinkedIn URLs when Yash provides them.
- P2: Add optional user-supplied audio files and real social URLs when available.
