# SoundSwitch Reference

This document aggregates the CSVs into easy-to-read Markdown tables for quick reference while building your SoundSwitch 2.10.1 project.

See also: `README_IMPORT.md` for import/patching steps and Control One mapping tips.

---

## Fixture Patch (Universe 1)

| Fixture | Manufacturer | Mode | Univ | Start |
|---|---|---|---:|---:|
| Showtec Phantom 65 Spot (1) | Showtec | 13ch | 1 | 1 |
| Showtec Phantom 65 Spot (2) | Showtec | 13ch | 1 | 14 |
| Showtec Phantom 65 Spot (3) | Showtec | 13ch | 1 | 27 |
| Showtec Phantom 65 Spot (4) | Showtec | 13ch | 1 | 40 |
| Showtec Phantom 65 Spot (5) | Showtec | 13ch | 1 | 53 |
| Showtec Phantom 65 Spot (6) | Showtec | 13ch | 1 | 66 |
| Cameo Nanobeam 600 (1) | Cameo | 14ch | 1 | 79 |
| Cameo Nanobeam 600 (2) | Cameo | 14ch | 1 | 93 |
| Showtec Shark Zoom Wash One (1) | Showtec | 15ch | 1 | 107 |
| Showtec Shark Zoom Wash One (2) | Showtec | 15ch | 1 | 122 |
| BeamZ LCB244 LED Bar (1) | BeamZ | 58ch | 1 | 137 |
| BeamZ LCB244 LED Bar (2) | BeamZ | 58ch | 1 | 195 |
| BeamZ LCB244 LED Bar (3) | BeamZ | 58ch | 1 | 253 |
| ADJ Sweeper Beam Quad LED (1) | ADJ | 39ch | 1 | 311 |
| ADJ Sweeper Beam Quad LED (2) | ADJ | 39ch | 1 | 350 |
| Martin THRILL Vertical Fogger | Martin | 7ch | 1 | 389 |
| BeamZ S1500LED Smoke Machine | BeamZ | 7ch | 1 | 396 |
| BeamZ SB200 LED Stage Blinder (1) | BeamZ | 6ch | 1 | 403 |
| BeamZ SB200 LED Stage Blinder (2) | BeamZ | 6ch | 1 | 409 |

Notes:
- Modes updated per your latest specs; addresses used: 001–414.

---

## Attribute Cues — Showtec Phantom 65 Spot

Use these as a programming checklist in the Attribute Editor (Color/Gobo/Prism/Frost/Focus/Strobe). Pair with stored positions for consistent looks.

| Cue Name | Color | Gobo | Prism | Frost | Focus | Strobe | Dimmer | Notes |
|---|---|---|---|---|---|---|---:|---|
| Open White (Sharp) | Open | Open | Off | Off | Sharp | Off | 100 | Baseline open white, sharp focus |
| Open White (Soft) | Open | Open | Off | On | Soft | Off | 100 | Soft wash using frost |
| Warm White Face | CTO | Open | Off | Off | Sharp | Off | 85 | Use CTO/Amber for speeches |
| Color: Deep Blue | Blue | Open | Off | Off | Sharp | Off | 100 | Solid color cue |
| Color: Red | Red | Open | Off | Off | Sharp | Off | 100 | Solid color cue |
| Color: Cyan | Cyan | Open | Off | Off | Sharp | Off | 100 | Solid color cue |
| Color: Magenta | Magenta | Open | Off | Off | Sharp | Off | 100 | Solid color cue |
| Gobo: Static 1 | Open | Gobo 1 Static | Off | Off | Sharp | Off | 95 | Textured static gobo |
| Gobo: Static 2 | Open | Gobo 2 Static | Off | Off | Sharp | Off | 95 | Alternate texture |
| Gobo: Rotate Slow | Open | Gobo 1 Rotate Slow | Off | Off | Sharp | Off | 95 | Slow rotation for ambience |
| Gobo: Rotate Fast | Open | Gobo 1 Rotate Fast | Off | Off | Sharp | Off | 95 | High energy moments |
| Prism: 3-Facet | Open | Open | 3-Facet | Off | Sharp | Off | 100 | Beam multiplication |
| Prism: 3-Facet + Rotate | Open | Gobo 1 Static | 3-Facet Rotate | Off | Sharp | Off | 100 | Rotating prism effect |
| Frost Wash | Open | Open | Off | On | Soft | Off | 100 | Wide soft wash from spots |
| Strobe: Slow | Open | Open | Off | Off | Sharp | 3 Hz | 100 | Ambient strobe |
| Strobe: Fast | Open | Open | Off | Off | Sharp | 10 Hz | 100 | Peak strobe |
| Beam Tight | Open | Open | Off | Off | Sharp | Off | 100 | Narrow beam, no frost |
| Beam Wide | Open | Open | Off | On | Soft | Off | 100 | Wide beam via frost |
| Focus Near | Open | Open | Off | Off | Near | Off | 100 | For near-field surfaces |
| Focus Far | Open | Open | Off | Off | Far | Off | 100 | For far-field projection |

---

## Position Presets

Store pan/tilt positions per fixture group; combine with the Attribute Cues above.

| Preset Name | Fixture Group | Description | Notes |
|---|---|---|---|
| Front Center | Phantom 65 Spots | Both heads centered front at eye-level tilt | Use for vocals/speeches |
| Front Split L/R | Phantom 65 Spots | One left to front-left, one right to front-right | Wide face coverage |
| Back Fan Wide | Phantom 65 Spots | Back wall fan with wide pan and medium tilt | Ambient texture |
| Back Fan Tight | Phantom 65 Spots | Back wall fan with tight pan and higher tilt | Sharper lines |
| Audience Sweep L→R | Phantom 65 Spots | Slow audience sweep from stage-left to stage-right | Automate with movement macro |
| Audience Sweep R→L | Phantom 65 Spots | Slow audience sweep from stage-right to stage-left | Automate with movement macro |
| Ceiling/Mirrorball | Phantom 65 Spots | Beams aimed at ceiling center/mirrorball | Use with prism/gobo for sparkle |
| Stage Corners UL | Phantom 65 Spots | Upper-left corner focus | For accents |
| Stage Corners UR | Phantom 65 Spots | Upper-right corner focus | For accents |
| Stage Corners DL | Phantom 65 Spots | Down-left corner focus | For accents |
| Stage Corners DR | Phantom 65 Spots | Down-right corner focus | For accents |
| Low Tilt Haze Cut | Phantom 65 Spots | Low tilt through haze above crowd | Wide frost optional |
| Far Wall Texture | Phantom 65 Spots | Far wall projection center | Use rotating gobo + slow |
| Center Spot (Speech) | Phantom 65 Spots | Single or pair centered for speech | CTO/Amber + sharp focus |
| DJ Booth Highlight | Phantom 65 Spots | Spotlights on DJ booth/performer | Use soft frost for camera |
| Dancefloor Center | Phantom 65 Spots | Beams converging at floor center | High energy moments |
| Entrance Ping | Phantom 65 Spots | Quick ping to venue entrance | For announcements |
| Back X Cross | Phantom 65 Spots | Crossed beams behind performer | Photo-friendly |
| Front Fan Wide | Shark Zoom Wash One | Wide fan to audience low tilt | Softer wash for dinner |
| Front Fan Tight | Shark Zoom Wash One | Tight fan higher tilt | Energy looks |
| Back Wash Halo | Shark Zoom Wash One | Back halo on performer | Low intensity |
| Dancefloor Wash | Shark Zoom Wash One | General floor coverage | Medium zoom |
| Beam Center | Nanobeam 600 | Center tight beams upwards | Use for build-ups |
| Beam Fan Wide | Nanobeam 600 | Wide beam fan to audience | Pair with strobe |
| Beam Sweep L→R | Nanobeam 600 | Sweep left to right | Narrow zoom |
| Beam Sweep R→L | Nanobeam 600 | Sweep right to left | Narrow zoom |
| Backline Accent | Nanobeam 600 | Accents for backline/branding | Static |

---

## Suggested Control One Mapping

- Pads: assign frequently used Phantom cues (Open White, Warm White Face, Deep Blue, Red, Static Gobo, Rotate Slow, 3‑Facet Prism)
- Encoders: map Color bank to encoder 1, Gobo to encoder 2, Prism/Focus to encoder 3/4 as preferred
- Buttons: Strobe button toggles Strobe Slow/Fast; Blackout reserved for speeches

If you want, I can also export this as PDFs for print, or expand with cue screenshots once you’ve set them in SoundSwitch.
