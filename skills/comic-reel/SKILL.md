---
name: "comic-reel"
description: "Make short comic comedy reels with animated gag scenes and pick from a catalog of 59 video styles (3D, anime, pixel, film, glitch and more)."
---

# Comic reel

Use this skill when the user asks for a comic reel, comedy scenes, a funny animated clip, or a set of video styles. Invoked as `/comic-reel` followed by a topic, for example `/comic-reel giant kid comedy scenes`.

## What to produce

1. A reel of 3 to 5 gag scenes about the user's topic, each 3 to 6 seconds, played in order with captions and a scene list.
2. Delivered as one self-contained HTML page (an artifact) with play and pause, a scrubber, scene jump buttons, and a clear first frame before play.
3. If the user asks for "styles", also show the same animation in several looks from the catalog below, as small looping tiles.

Be honest in the reply: these are in-page animations and procedural style filters, not rendered video files or real output from 3D, anime or film tools. For an MP4, the user can screen-record the player.

## Writing a gag scene

Each scene is one joke with three beats.

- Setup (about 1 s): show the situation and the character clearly.
- Escalation (about 2 s): one visual action that makes the problem obvious.
- Punchline (about 1 to 2 s): a sound-word pop (BONK, THUD, ACHOO) or a short speech bubble that lands the joke.

Rules for the jokes:

- Keep one idea per scene. Use scale, mismatch or rule-of-three for the humor.
- Write captions in plain words, at most about 18 words, so they can be read aloud in the scene length.
- Keep characters friendly. No jokes that target real people or groups.
- Reuse a small cast (hero, a tiny friend, one prop) across scenes so the reel feels like one world.

## Building it

- Drive every animation from one timeline value so scrubbing and replay always match.
- Use SVG with CSS keyframes for 2D scenes, or three.js for 3D scenes. Respect reduced motion.
- Design for phone width. Provide light and dark page themes.
- Include a poster frame so the page is complete before the user presses play.

## Style catalog (59)

When a style is requested, apply it as the look of the whole reel. Name the style and its frame rate in the caption area.

**3D (8):** 1 Low-poly 3D (triangle facets), 2 Voxel world (bevelled blocks), 3 Brick toy (studs, gaps), 4 Cel-shaded 3D (posterize plus ink edge), 5 Claymation (8 fps, wobble, soft), 6 Soft CGI (bloom, warm grade), 7 Hologram (cyan scanlines, flicker), 8 Wireframe (green edges on black).

**Anime (7):** 9 Anime cel (flat shading, ink line, sparkles), 10 Shonen speed lines, 11 Manga halftone (black and white dots), 12 80s OVA anime (soft, warm, grain), 13 Chibi pastel, 14 Magical girl (pink purple glow, stars), 15 Studio watercolor (hand-painted soft).

**Cartoon (9):** 16 Crayon, 17 Rubber hose 1930s (gray, bouncy, scratches), 18 Saturday cartoon (bright, thick ink), 19 Pop-art comic (Ben-Day dots), 20 Newspaper strip (gray dots on newsprint), 21 Flipbook (8 fps, page border), 22 Rotoscope (boiling lines), 23 Paper cut-out (jerky, flat), 24 Warhol four-up.

**Painted and craft (12):** 25 Watercolor, 26 Oil painting, 27 Ukiyo-e woodblock, 28 Sumi-e ink wash, 29 Stained glass, 30 Mosaic tiles, 31 Cross-stitch, 32 Pencil sketch, 33 Chalkboard, 34 Blueprint, 35 Pointillism, 36 Risograph (two-ink misregistered print).

**Retro games (8):** 37 Game Boy (4 greens), 38 NES 8-bit, 39 16-bit console, 40 Commodore 64, 41 CGA computer (cyan, magenta, white, black), 42 ASCII terminal, 43 LED matrix, 44 Vector arcade (glowing white lines).

**Film and camera (9):** 45 Silent film (sepia, scratches, pillarbox), 46 Film noir (blinds light), 47 VHS tape (tracking band, chroma shift), 48 Security cam (timestamp), 49 Found footage (shaky, REC), 50 Cinematic teal-orange (letterbox), 51 Night vision, 52 Thermal camera, 53 Fisheye action cam.

**Digital (6):** 54 Glitch art, 55 Datamosh (smear trails), 56 Pixel sort, 57 Vaporwave, 58 Synthwave (neon grid), 59 Neon sign.

## Reply format

One or two sentences: what the reel is, which style it uses, and the honest note about it not being a video file. No recap of the steps.