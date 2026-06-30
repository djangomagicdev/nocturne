# NOCTURNE

*a moonlit dreamscape that writes its own music*

→ **https://djangomagicdev.github.io/nocturne/**

An endless, slowly-mutating surreal dreamscape that opens the moment the page loads: a
GPU-rendered horizon of flowing mist and a sky that drifts through colour beneath a pale moon,
scored by generative ambient music synthesized live in the browser. No two minutes are ever the
same, and the dream is seeded fresh each day.

Nothing to read, nothing to fill in. Just drift.

### Be there

Best **fullscreen, with sound on, in a dark room.**

- **Move the cursor** to part the mist — the whole scene parallaxes with you.
- **Click anywhere** to cast a stone — a ripple crosses the sky and a single bell sounds.
- **Spacebar** mutes / unmutes.

**Sound:** it plays automatically wherever the browser allows it. On a brand-new first visit some
browsers block autoplay, so the score fades in the instant you click or press a key — and after
that it just starts on its own.

### Under the hood

One self-contained HTML file — no dependencies, no build step, nothing to install. A WebGL2
fragment shader (domain-warped fractal noise) paints the dreamscape; the Web Audio API
synthesizes the ambient score live, scheduled note by note. The audio engine is the conductor:
each chord change pushes colour and light into the sky, so image and sound breathe as one. It
degrades gracefully — a Canvas2D fallback where WebGL isn't available, muted-but-beautiful where
audio is blocked, and a calmer path for reduced-motion.

🌙
