# ROBIN

## UNDER REVIEW
check for updates when published

## DJ + Lighting Setup

This section provides:
- Links to Denon DJ and related software downloads
- A complete example spec for a DJ rig with lighting
- Cable list with quantities and provided lengths
- DMX addressing plan and setup notes

---

### Denon DJ Software and Resources
- Engine DJ Desktop (music library prep): https://enginedj.com/downloads
- Engine DJ Desktop (direct page): https://enginedj.com/software/enginedj-desktop
- Engine DJ OS Updates (on-controller firmware): https://enginedj.com/downloads
- Denon DJ Product Downloads (firmware, manuals): https://www.denondj.com/downloads
- SoundSwitch (lighting control, integrates with Engine Lighting): https://www.soundswitch.com/download
- Engine Lighting (SoundSwitch integration overview): https://enginedj.com/lighting
- Denon DJ Knowledge Base: https://support.inmusicbrands.com/hc/en-us/categories/360002590432-Denon-DJ

Tip: With compatible Denon DJ controllers/players, Engine Lighting lets you run SoundSwitch lighting shows directly from the hardware without a laptop.

---

### System Overview
- DJ Booth: Denon DJ X1850 Prime + 2x SC5000M Prime (flight case)
- Audio: 2x Bose F1 Model 812 + 2x Bose F1 Subwoofer
- Lighting:
    - 6x Showtec Phantom 65 Spot
    - 2x Cameo Nanobeam 600
    - 2x Showtec Shark Zoom Wash One RGBW LED moving heads
    - 3x BeamZ LCB244 LED Bars
    - 1x Martin THRILL Vertical Fogger
    - 1x BeamZ S1500LED Fog Machine (1500W, DMX + LEDs)
    - 2x ADJ Sweeper Beam Quad LED
- Control: SoundSwitch Control One (integrated DMX)
- Storage: SC5000M includes a 1 TB internal drive for the Engine DJ music library
- Network: Netgear GS108 8‑port Gigabit switch linking X1850 and SC5000M players (and laptop if required)
- Power: Dedicated power distribution with surge/RCD, proper gauge cables, tidy cable runs
- Truss: 2x truss sections 200 x 30 cm with cover sleeves and top/bottom plates

---

### Example Bill of Materials (BOM)

#### DJ and Audio
- Mixer: Denon DJ X1850 Prime
- Media Players: 2x Denon DJ SC5000M Prime (motorized platters), with 1 TB internal drive installed for onboard library
- PA: 2x Bose F1 Model 812 Flex Array (active) + 2x Bose F1 Subwoofer (active)
- Microphones: 1x Shure SM7dB dynamic (XLR, built-in preamp; use 48V phantom when preamp is enabled); 1x Sennheiser XS 1 dynamic (XLR; no phantom required)
- Utility Mixer/USB Audio: Behringer XENYX 1204USB (for mic routing, recording, or additional sources)
- Headphones: Pioneer DJ HDJ-X10 (Black)

#### Lighting Fixtures
- Moving Head Spots: 6x Showtec Phantom 65 Spot (65W LED), 16-bit pan/tilt, gobo + color wheel, 8–16 channels (mode dependent)
- Moving Beam Heads: 2x Cameo Nanobeam 600 (beam), 8–16 channels (mode dependent)
- Moving Wash Heads: 2x Showtec Shark Zoom Wash One RGBW LED (motorized zoom wash), 8–16 channels (mode dependent)
- LED Bars: 3x BeamZ LCB244 LED Bar (24x 4W RGBW), typical 16-ch mode supported
- Fog: 1x Martin THRILL Vertical Fogger (vertical CO2-style effect), use manufacturer-recommended fluid
 - Fog: 1x BeamZ S1500LED Fog Machine (1500W, DMX + LEDs), use manufacturer-recommended fluid
 - Effects Bars: 2x ADJ Sweeper Beam Quad LED (RGBW, multi-mode including pixel control)

Safety note: Verify local regulations for haze/fog and laser use. Avoid audience scanning with lasers; prefer no-laser rigs for mobile events.

#### Control and Rigging
- DMX Interface: SoundSwitch Control One (integrated dual DMX outputs)
- Truss: 2x truss sections 200 x 30 cm with white cover sleeves and top/bottom plates (use rated bases and secure with safety)
- Cases: 2x flight cases for Showtec moving heads
- Network: Netgear GS108 8‑port Gigabit switch

Additional control hardware:
- SoundSwitch Control One USB hardware for hands-on control of Autoloops, Static Looks, Strobe/Blinder, Smoke, Blackout, and next/previous scene selection.

---

### Kit Contents (What You Receive)
- Flight Case (DJ players + mixer): X1850 Prime mixer + 2x SC5000M Prime media players
- PA: 2x Bose F1 Model 812 Flex Array loudspeakers + 2x Bose F1 Subwoofer
- Microphones: 1x Shure SM7dB (wired), 1x Sennheiser XS 1 (wired)
- Utility: Behringer XENYX 1204USB (USB mixer)
- Lighting:
  - 6x Showtec Phantom 65 Spot
  - 2x Cameo Nanobeam 600
  - 2x Showtec Shark Zoom Wash One RGBW LED moving heads
  - 3x BeamZ LCB244 LED Bars
  - 1x Martin THRILL Vertical Fogger
  - 1x BeamZ S1500LED Fog Machine (1500W, DMX + LEDs)
  - 2x ADJ Sweeper Beam Quad LED
- Control: SoundSwitch Control One (USB)
- Network: Netgear GS108 8‑port Gigabit switch + Cat5e/Cat6 patch cables
- Truss: 2x truss sections 200 x 30 cm with white cover sleeves and top/bottom plates
- Cases: 2x flight cases for Showtec moving heads
 - Headphones: Pioneer DJ HDJ-X10 (Black)
 - Storage: 1 TB internal drive installed in SC5000M for onboard library

If any item is missing or damaged, stop and contact the equipment provider before proceeding.

---

### Cabling and Power
TBD — Cables list will be added later.

---

### Network Connectivity
- Place the Netgear GS108 switch near the X1850.
- Connect X1850 Ethernet to GS108 (any port).
- Connect both SC5000M players’ Ethernet to GS108.
- Optional: connect a laptop to GS108 for Engine DJ Desktop/updates if needed.
- Use Cat5e/Cat6 cables. No special IP setup is required; devices auto‑link.

---

### DMX Layout (Example)
- Universe: 1 (512 channels)
- Addressing plan:
  - Moving Head 1: start 001 (16 ch)
  - Moving Head 2: start 017 (16 ch)
  - Moving Head 3: start 033 (16 ch)
  - Moving Head 4: start 049 (16 ch)
  - Moving Head 5: start 065 (16 ch)
  - Moving Head 6: start 081 (16 ch)
  - Moving Beam 1: start 097 (16 ch)
  - Moving Beam 2: start 113 (16 ch)
  - Moving Wash 1: start 129 (16 ch)
  - Moving Wash 2: start 145 (16 ch)
  - LED Bar 1: start 161 (16 ch)
  - LED Bar 2: start 177 (16 ch)
  - LED Bar 3: start 193 (16 ch)
  - Effects Bar 1 (Sweeper): start 209 (16 ch)
  - Effects Bar 2 (Sweeper): start 225 (16 ch)
  - Fog 1 (Martin THRILL): start 241 (2 ch)
  - Fog 2 (BeamZ S1500LED): start 243 (2 ch)
- Terminate the last fixture in the chain with a 120 Ω terminator.

Note: If using Engine Lighting with SoundSwitch, you can auto-generate shows from track metadata and BPM, and map fixtures via Fixture Profiles. Ensure all fixture profiles exist in the SoundSwitch library.

---

### Setup Checklist
- Update Engine OS and Engine DJ Desktop to latest versions
- Enable Engine Lighting and test basic looks (static, auto, and strobe)
- Patch all fixtures in SoundSwitch and verify addressing matches physical rig
- Soundcheck: gain staging, limiters, and crossover settings on subs/tops
- Safety: secure all fixtures with safety bonds; tape or ramp all floor cables; RCD in-use
- Label all cables and pack by length/type for faster teardown

---

### How to Run the Rig (Step-by-Step)

### 1) Pre‑Event Preparation
1. Prepare the SM7dB and confirm phantom power (if using built-in preamp) on the mixer/interface.
2. Prepare the Sennheiser XS 1 and connect via XLR.
3. Update Engine OS on the controller and Engine DJ Desktop if needed.
4. Sync your Engine DJ library to the SC5000M’s internal 1 TB drive (or to your performance USB) and verify playlists load.
5. Open SoundSwitch and verify the venue/light show project. Export show data to the Engine drive if using Engine Lighting.
6. Label cable bundles by length (short/medium/long) and fixture groups.

### 2) Room Layout and Power
1. Place DJ booth where power is available and safe from foot traffic/spills.
2. Position PA: place Bose F1 subs and tops left/right of dance floor, slight toe-in.
3. Position truss to left/right of booth. Ensure overhead clearance; secure fixtures with safety bonds.
4. Run a dedicated power run to audio and a separate one to lighting where possible to reduce noise.
5. Use RCD/RCBO protection. Keep cables along walls; cross walkways with cable ramps.
6. Place GS108 switch near the mixer and connect Ethernet to X1850 and SC5000M units (optional laptop to GS108).

### 3) Build Audio
1. Place subs and tops. Power off everything.
2. Connect controller master out to subs (XLR L/R). From subs’ high-pass outs to tops (XLR L/R).
3. Connect booth out to booth monitors (TRS/XLR).
4. Connect microphone(s): SM7dB via XLR to mixer input (enable phantom if using built-in preamp); XS 1 via XLR (no phantom required).
5. Power on sequence: controller → subs → tops → booth monitors.
6. Set initial gains: controller master at 0 dB, channel gains to unity, subs/tops input gains noon; limiters on.

Using XENYX 1204USB (optional):
- Route mics into XENYX channels; send XENYX main outs to X1850 line inputs (L/R) for FOH.
- Or use XENYX USB to record the event on a laptop; set the USB routing per the manual.

Bose F1 wiring (recommended):
- Connect X1850/Controller Master L/R to Bose F1 Subwoofer L/R inputs.
- From each Sub, connect HPF/Thru Out to the corresponding F1 Model 812 input (L → Left, R → Right).
- On the Sub, set HPF to engage the internal crossover; start with Sub level at 12 o’clock; adjust during soundcheck.
- On the 812 tops, set input level around 12 o’clock; select array pattern to suit coverage; fine-tune during soundcheck.

### 4) Build Lighting (DMX)
1. With power off, mount fixtures on T-bars/truss using rated clamps and safety bonds.
2. Daisy-chain DMX from Control One DMX out to first fixture, then through the chain.
3. Set fixture DMX addresses to match the DMX Layout table above; set DMX mode/channel count per the plan.
4. Plug in power to each fixture. Use IEC/PowerCON as applicable. Keep DMX and power separated where possible.
5. Place a DMX terminator at the last fixture in the chain.

### 5) Engine Lighting / SoundSwitch Setup
Option A: Engine Lighting (no laptop during show)
- In controller settings, enable Engine Lighting.
- Insert the Engine/SoundSwitch USB drive. Load a track and open Lighting view to verify looks.
- Select venue/show profile if prompted. Test static, color, movement, and strobe looks.

Note: SoundSwitch Control One requires a laptop running SoundSwitch software.

Option B: Laptop with SoundSwitch + Control One
- Connect Control One to the laptop via USB. In SoundSwitch, verify Control One is detected (and set as the DMX interface if using its outputs).
 - If not using Control One DMX outputs, select your USB DMX interface in preferences.
- Open your show project, confirm fixtures are patched/profiled, and addresses match hardware.
- Use Control One pads/encoders:
  - Autoloops: trigger and adjust intensity/color/movement banks
  - Static Looks: select static scenes for dinner/speeches
  - Strobe/Blinder/Smoke: dedicated buttons
  - Blackout: master blackout toggle
  - Next/Previous: step through programmed looks
- Start Autoloops or trigger scripted shows. Verify output on fixtures.

### 6) Soundcheck
1. Play a reference track at performance level. Adjust sub/top input gains and crossover as needed.
2. Walk the room. Balance left/right and sub/top levels. Avoid clipping; keep headroom.
3. Check mics for feedback; apply HPF and moderate EQ on the controller.
4. Confirm lighting reacts to BPM and looks appropriate for the venue.

### 7) During the Event
- Keep controller master around 0 dB; use channel faders and EQ for mixing.
- Use Booth level to control your monitor volume independently.
- For lighting, toggle between Autoloops/Static Scenes for slow songs vs energetic looks for peak moments.
- Use blackout for speeches or as needed; avoid excessive strobe.

### 8) Teardown and Packing
1. Power down sequence: booth monitors → tops → subs → controller → lighting fixtures.
2. Remove DMX terminator; coil DMX and audio cables with over-under technique; velcro and bag by length.
3. Remove fixtures; keep clamps and safety bonds with each fixture case.
4. Pack controller, mics, and accessories. Verify all items against Packing Checklist.
5. Inspect the area; remove tape and cable ramps.

---

## Troubleshooting Quick Guide
- No sound from tops: check master output routing, sub high-pass outs, input gains, and mute/limit LEDs.
- Hum/buzz: separate audio and lighting power, use balanced cables, lift ground on DI (not on mains!).
- No DMX response: verify addresses/mode, DMX polarity, terminator in place, and interface selected.
- Flickering lights: replace suspect DMX cable, check terminator, reduce cable run length if possible.
- Engine Lighting not working: confirm Engine Lighting enabled and SoundSwitch data on the drive.

---

## Packing Checklist (Return in Good Order)
- X1850 + 2x SC5000M flight case + PSU, USB engine drive
- 2x Bose F1 Model 812 + 2x Bose F1 Subwoofer
- 6x Showtec Phantom 65 Spot, 2x Cameo Nanobeam 600, 2x Showtec Shark Zoom Wash One RGBW LED, 3x BeamZ LCB244 LED Bars, 2x ADJ Sweeper Beam Quad LED, 1x Martin THRILL Vertical Fogger, 1x BeamZ S1500LED
- SoundSwitch Control One, 2x DMX terminators
- Cables: TBD (full list to be added later)
- Truss: 2x 200 x 30 cm with sleeves and plates
- Cases: 2x flight cases for Showtec moving heads
- Microphones: Shure SM7dB, Sennheiser XS 1
 - Headphones: Pioneer DJ HDJ-X10 (Black)
- Netgear GS108 Gigabit Switch

---

### Quick Links
- Engine DJ Downloads: https://enginedj.com/downloads
- SoundSwitch Downloads: https://www.soundswitch.com/download
- Denon DJ Support: https://support.inmusicbrands.com/hc/en-us/categories/360002590432-Denon-DJ
- SoundSwitch Control One: https://www.soundswitch.com/hardware/control-one
- Bose F1 Model 812: https://www.bax-shop.nl/actieve-fullrange/bose-f1-model-812
- Bose F1 Subwoofer: https://www.bax-shop.nl/actieve-subwoofer/bose-f1-subwoofer-actief
- Showtec Phantom 65 Spot: https://www.bax-shop.nl/led-moving-head/showtec-phantom-65-spot-led-movinghead
- Martin THRILL Vertical Fogger: https://www.gear4music.nl/nl/PA-DJ-and-Verlichting/Martin-THRILL-Verticale-Fogger/25YE
- Cameo Nanobeam 600: https://www.cameolight.com/en/solutions/dj-musicians/moving-lights/moving-heads/20447/nanobeam-600
- BeamZ LCB244 LED Bar: https://www.beamzlighting.com/product/lcb244-led-bar-24x-4w/
- BeamZ S1500LED Fog Machine: https://www.maxiaxi.com/beamz-s1500led-rookmachine-met-dmx-en-led-s-1500-watt/
- Sennheiser XS 1: https://www.bax-shop.nl/dynamische-zangmicrofoons/sennheiser-xs-1-dynamische-microfoon
- Shure SM7dB: https://www.bax-shop.nl/dynamische-zang-microfoons/shure-sm7db-dynamische-studiomicrofoon-met-ingebouwde-preamp
  - ADJ Sweeper Beam Quad LED: https://www.adj.eu/sweeper-beam-quad-led
  - Behringer XENYX 1204USB: https://www.behringer.com/product.html?modelCode=0601-ACM
  - Netgear GS108 Gigabit Switch: https://www.netgear.com/business/wired/switches/unmanaged/gs108/
- Showtec Shark Zoom Wash One RGBW LED: https://www.bax-shop.nl/led-moving-head/showtec-shark-zoom-wash-one-rgbw-led-movinghead
- Pioneer DJ HDJ-X10 (Black): https://www.pioneerdj.com/en/product/headphones/hdj-x10/black/overview/
