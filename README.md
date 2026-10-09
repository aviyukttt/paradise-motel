# Paradise Motel — Lana Del Rey Record Room

A cinematic, responsive record-player experience built around the supplied cathedral and Lana CD artwork. Browse the official-release catalog, filter by era, choose a record, watch it find the player, and use the transport controls to drive the visual listening state.

## Run locally

```bash
npm start
```

Then open `http://localhost:3000`.

## Audio behavior

The Play button now starts an audible vinyl-scratch preview generated with the Web Audio API and drives a custom canvas equalizer. The same user gesture opens the selected track’s official Spotify search page so the copyrighted recording can be heard from the licensed service. The repository does not host or redistribute Lana Del Rey recordings, so the site cannot legally stream the songs directly from its own server.

## What is included

The site uses a full-bleed cathedral background, the supplied Lana CD artwork, glassmorphic panels, a CSS-built turntable, a disc insertion animation, GSAP + ScrollTrigger reveals, album filters, a 114-entry official-release metadata catalog, keyboard controls, seek/volume controls, a Web Audio scratch effect, a live equalizer visualizer, and responsive desktop/mobile layouts.

## Credits and asset note

The supplied image assets are included for this project. Lana Del Rey song titles and album metadata are used for catalog/navigation purposes; the recordings remain on their official streaming services.
