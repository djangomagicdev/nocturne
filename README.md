# NOCTURNE

*a dream you fall into, that quietly forgets you back*

A single, self-contained web page that opens into an endless, slowly-mutating surreal
dreamscape — a GPU-rendered horizon of flowing mist and a migrating sky beneath a pale moon,
scored by generative ambient music synthesized live in the browser, and narrated by drifting
fragments of dream-poetry. You don't play it. You drift through it, and it never repeats.

It begins by asking you one question — *what do you not want to forget?* — and the words you
type become the seed of the whole dream: its colours, its musical key, and a single recurring
line of poetry that, over the minutes you stay, slowly and visibly **forgets itself**.

The same words always summon the same dream, so a dream is shareable: tell someone the memory
you typed and they'll fall into the same colours, the same key, the same drifting line.

### Be there

Best experienced **fullscreen, with sound on, in a dark room.**

- **Type a memory and press Enter** to summon your dream — or leave it empty to simply drift.
- **Move the cursor** to part the mist.
- **Click** to cast a stone — a ripple crosses the sky and a single bell sounds.
- **Spacebar** mutes / unmutes.

### Under the hood

Vanilla HTML/CSS/JS in one file — no dependencies, no build step. A WebGL2 fragment shader
(domain-warped fractal noise) paints the dreamscape; the Web Audio API synthesizes the score
live; a hand-written grammar writes the poetry. The audio engine is the conductor: each chord
change pushes colour and light into the sky and sets the cadence of the words, so image, sound,
and language move as one. It degrades gracefully (Canvas2D fallback, muted-but-beautiful with no
audio, reduced-motion).

🌙
