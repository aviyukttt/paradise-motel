# Paradise Motel — Lana Del Rey Record Player

## Implementation

A dependency-light static web experience served on port 3000. The app uses one semantic HTML page, CSS custom properties, and vanilla JavaScript. GSAP + ScrollTrigger are loaded from pinned CDN URLs for the disc-insertion sequence, ambient drift, and scroll-linked catalog reveals. The supplied `ParadiseMotelCoastalDaydream.png` is copied into `public/assets/` and used as the full-page background. The catalog is metadata-only and routes listeners to official Spotify search pages; the project does not redistribute copyrighted recordings.

## Design direction

- **Design movement:** cinematic glassmorphism / nocturnal Americana record lounge.
- **Core principles:** immersive but readable, tactile controls, editorial song browsing, slow-burn motion.
- **Color philosophy:** sepia candlelight and burgundy echo the supplied motel-at-sunset artwork; near-black overlays preserve contrast; pearl text feels like printed liner notes.
- **Layout paradigm:** asymmetric editorial composition: a slim masthead, a central hero/player stage, and a lower horizontal record shelf instead of a dashboard grid.
- **Signature elements:** rotating vinyl grooves, red playhead glow, tiny liner-note labels and a translucent motel-sign badge.
- **Interaction philosophy:** selecting a record feels like placing it on a turntable; every meaningful action has a visible physical response.
- **Animation:** 700ms–1.4s ease-out transitions, subtle continuous record rotation while active, staggered catalog reveals via ScrollTrigger, no motion that blocks controls.
- **Typography:** Playfair Display for titles and serif editorial copy; DM Sans for controls, labels and metadata.
- **Brand essence:** a quiet digital record room for late-night Lana listening — intimate, tactile, transportive. Personality: smoky, romantic, considered.
- **Brand voice:** headlines are evocative but concise; microcopy is calm and useful. Examples: “Choose a side of the night.” / “The needle is waiting.”
- **Wordmark:** PARADISE MOTEL set as a small uppercase wordmark with a thin red vertical line, like a motel key tag.
- **Signature brand color:** motel neon red `#c75c57`.

## Project structure

- `index.html` — page structure, catalog data, filtering, player state and interaction logic.
- `styles.css` — responsive visual system, player, records and motion-safe states.
- `server.mjs` — minimal static server with SPA fallback and port support.
- `public/assets/ParadiseMotelCoastalDaydream.png` — user-supplied background artwork.
- `public/manus-routes.json` — route manifest required by the hosted preview.
- `README.md` — setup, content/licensing and publishing notes.

## Material constraints

The site includes the complete official studio/EP track metadata represented in the interface, but it does not host or stream copyrighted Lana Del Rey audio files. The “play” interaction performs the visual loading/needle-drop experience, updates a simulated progress bar, and provides an official Spotify search handoff for the selected song.
