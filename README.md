  # Multiplayer Shiritori (2-Player, Same Screen)

  A minimal, dependency‑free browser game implementing Shiritori with:
  - Turn‑based play with auto turn switch
  - Dictionary validation via dictionaryapi.dev
  - Structure rules: start letter must match previous word's last letter, >= 4 letters, no repeats
  - Per‑turn countdown timer
  - Score tracking (+1 valid, −1 invalid/timeout)
  - Word history with meanings
  - Deployed easily as a static site (Netlify/Vercel)

  ## Quick Start
  1. Put this `index.html` in a repo.
  2. Open in a browser to play locally — or deploy to Netlify/Vercel as a static site.

  ## Scoring Rules
  - ✅ Valid word: +1 point for the current player.
  - ❌ Invalid submission (fails rules or not found) or ⏱️ timeout: −1 point and turn passes.

  ## Tech Notes
  - No build step required. No external libs. Uses fetch to `https://api.dictionaryapi.dev/api/v2/entries/en/<word>`.
  - Caches meanings in memory during the session.

  ## Folder Structure
  - Single file: `index.html` (contains HTML, CSS, JS). Optional: extract JS/CSS later.

  ## Accessibility & UX
  - Keyboard: Enter to submit; `Tab` navigable; focus returned to input each turn.