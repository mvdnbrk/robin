# ROBIN

## UNDER REVIEW

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
- DJ Booth: Denon DJ controller with Engine DJ and Engine Lighting enabled
- Audio: 2x tops + 1–2x subs, booth monitors, mics
- Lighting: Moving heads, LED PAR wash, LED bar effects, strobe/blinder, haze (venue permitting)
- Control: Engine Lighting via SoundSwitch, or SoundSwitch Control One (integrated DMX)
- Power: Dedicated power distribution with surge/RCD, proper gauge cables, tidy cable runs
- Stands/Truss: Two lighting stands with a crossbar or a short truss span

---

### Example Bill of Materials (BOM)

#### DJ and Audio
- Controller: Denon DJ PRIME series (e.g., PRIME 4 / SC LIVE 4 / SC LIVE 2) with latest Engine OS
- Laptop (optional): For library prep in Engine DJ Desktop and SoundSwitch show creation
- PA Tops: 2x 12" or 15" powered speakers (e.g., 1000–2000 W peak each)
- Subwoofers: 1–2x 15" or 18" powered subs (1000–2000 W peak each)
- Booth Monitors: 2x compact powered speakers (8"–10")
- Microphones: 1x wired dynamic (XLR) + 1x wireless handheld kit (UHF/2.4 GHz per local regulation)
- DI/Utility: 1x stereo DI box (for venue tie-ins) + ground lift switches
- Audio Management: Optional 2x2 USB interface if recording, or small utility mixer if multiple sources

PA Option (Bose F1 system):
- 2x Bose F1 Model 812 Flex Array loudspeakers (active)
- 2x Bose F1 Subwoofer (active)

Alternative club setup (flight case):
- Mixer: Denon DJ X1850 Prime
- Media Players: 2x Denon DJ SC5000M Prime (motorized platters)

#### Lighting Fixtures
- Moving Head Spots: 6x Showtec Phantom 65 Spot (65W LED), 16-bit pan/tilt, gobo + color wheel, 8–16 channels (mode dependent)
- LED Wash PARs: 8x RGBW or RGBA 10–12W x7 LEDs, 6–10 channels
- LED Bars (effects/wash): 2x pixel-mappable RGB bars, 8–24 channels
- Strobe/Blinder: 2x LED strobe/blinder combo, 4–8 channels
- Hazer: 1x water-based haze machine, DMX-capable
- Wireless DMX (optional): 1x transmitter + 3–4x receivers, or use cabled DMX

Safety note: Verify local regulations for haze/fog and laser use. Avoid audience scanning with lasers; prefer no-laser rigs for mobile events.

#### Control and Rigging
- DMX Interface: SoundSwitch Control One (integrated dual DMX outputs) or SoundSwitch USB-to-DMX interface
- Lighting Stands: 2x tripod stands with T-bars or 2x crank stands + 2–3 m truss (verify load rating for 6 moving heads)
- Clamps: 20–24x O-clamps or trigger clamps (rated for fixture weight)
- Safety Bonds: 20–24x steel safety cables, rated
- Cases: Controller case, cable trunk, fixture bags/cases

Additional control hardware:
- SoundSwitch Control One USB hardware for hands-on control of Autoloops, Static Looks, Strobe/Blinder, Smoke, Blackout, and next/previous scene selection.

---

### Cabling and Power

#### Audio Cables
- XLR(M–F) balanced
  - 2x 10 m for tops
  - 2x 2–5 m for booth monitors
  - 2x 5–10 m from controller/mixer to subs (if subs handle crossover)
- TRS 1/4" balanced
  - 2x 1–3 m utility patch
- RCA
  - 1x 1–2 m backup/aux input cable

#### DMX Cables (110–120 Ω, not audio XLR)
- 3-pin or 5-pin based on fixtures
  - 2x 10 m main runs
  - 10x 5 m fixture links
  - 6x 1–2 m short patch leads
- DMX Terminators
  - 2x 120 Ω terminators for end-of-line

#### Power Cables
- Mains Extensions (region-specific plugs)
  - 2x 10–15 m
  - 4x 5 m
- IEC C13/C14
  - 8–12x 2–3 m for fixtures and speakers
- PowerCON (if your speakers/fixtures use them)
  - 2–4x 3–5 m
- Power Distribution
  - 2x 6–8 outlet power strips with surge/RCD where required
  - 1x small rack/box distro (optional) with MCBs/RCDs per local code

Cable management: Velcro ties, cable ramps for walkways, gaffer tape (residue-free), and labeled ends.

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
  - LED Bar 1: start 097 (16 ch)
  - LED Bar 2: start 113 (16 ch)
  - PARs 1–4: start 129, 137, 145, 153 (8 ch each)
  - PARs 5–8: start 161, 169, 177, 185 (8 ch each)
  - Strobe/Blinder 1–2: start 193, 201 (4–8 ch each)
  - Hazer: start 209 (2 ch)
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

## Kit Contents (What You Receive)
- Controller: Denon DJ PRIME-series controller with power supply
- Flight Case (DJ players + mixer, alternative to all-in-one controller): X1850 Prime mixer + 2x SC5000M Prime media players
- PA: 2x Bose F1 Model 812 Flex Array loudspeakers + 2x Bose F1 Subwoofer, 2x booth monitors
- Lighting: 6x moving heads (Showtec Phantom 65 Spot), 8x PARs, 2x LED bars, 2x strobe/blinders, 1x hazer
- Control: SoundSwitch Control One (USB) with integrated dual DMX outputs (USB cable included), or wireless DMX kit; SoundSwitch project USB
- Stands/Truss: 2x lighting stands with T-bars or mini truss
- Cabling: Audio XLR/TRS, DMX (3/5-pin), mains, IEC/PowerCON, DMX terminators
- Accessories: Clamps, safety bonds, power strips with RCD/surge, tape, cable ties
- Cases: Marked for controller, cables, audio, lighting

If any item is missing or damaged, stop and contact the equipment provider before proceeding.

---

## How to Run the Rig (Step-by-Step)

### 1) Pre‑Event Preparation
1. Charge wireless mic(s) and check batteries/spares.
2. Update Engine OS on the controller and Engine DJ Desktop if needed.
3. Export your Engine DJ library to the performance USB/drive. Verify playlists load.
4. Open SoundSwitch and verify the venue/light show project. Export show data to the Engine drive if using Engine Lighting.
5. Label cable bundles by length (short/medium/long) and fixture groups.

### 2) Room Layout and Power
1. Place DJ booth where power is available and safe from foot traffic/spills.
2. Position PA: subs on floor, tops on stands left/right of dance floor, slight toe-in.
3. Place lighting stands to left/right of booth. Ensure overhead clearance; use safety bonds.
4. Run a dedicated power run to audio and a separate one to lighting where possible to reduce noise.
5. Use RCD/RCBO protection. Keep cables along walls; cross walkways with cable ramps.

### 3) Build Audio
1. Place subs and tops. Power off everything.
2. Connect controller master out to subs (XLR L/R). From subs’ high-pass outs to tops (XLR L/R).
3. Connect booth out to booth monitors (TRS/XLR).
4. Connect microphones: wireless receiver via XLR to controller/mixer; wired mic to XLR input.
5. Power on sequence: controller → subs → tops → booth monitors.
6. Set initial gains: controller master at 0 dB, channel gains to unity, subs/tops input gains noon; limiters on.

Bose F1 wiring (recommended):
- Connect X1850/Controller Master L/R to Bose F1 Subwoofer L/R inputs.
- From each Sub, connect HPF/Thru Out to the corresponding F1 Model 812 input (L → Left, R → Right).
- On the Sub, set HPF to engage the internal crossover; start with Sub level at 12 o’clock; adjust during soundcheck.
- On the 812 tops, set input level around 12 o’clock; select array pattern to suit coverage; fine-tune during soundcheck.

### 4) Build Lighting (DMX)
1. With power off, mount fixtures on T-bars/truss using rated clamps and safety bonds.
2. Daisy-chain DMX from controller/USB DMX or wireless receiver to first fixture, then through the chain.
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
- If not using Control One DMX outputs, select your USB DMX or wireless interface in preferences.
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
- Controller + PSU, USB engine drive
- 2x tops, 1–2x subs, 2x booth monitors
- 2x moving heads, 8x PARs, 2x LED bars, 2x strobe/blinders, hazer
- DMX interface or wireless kit, 2x DMX terminators
- Audio cables: XLR, TRS, RCA as listed
- DMX cables: long, medium, short bundles
- Power: extensions, IEC/PowerCON, power strips with RCD
- Clamps, safety bonds, tape, ties, tools
- Microphones (wired + wireless), spare batteries

---

### Quick Links
- Engine DJ Downloads: https://enginedj.com/downloads
- SoundSwitch Downloads: https://www.soundswitch.com/download
- Denon DJ Support: https://support.inmusicbrands.com/hc/en-us/categories/360002590432-Denon-DJ
- SoundSwitch Control One: https://www.soundswitch.com/hardware/control-one
- Bose F1 Model 812: https://www.bax-shop.nl/actieve-fullrange/bose-f1-model-812
- Bose F1 Subwoofer: https://www.bax-shop.nl/actieve-subwoofer/bose-f1-subwoofer-actief
- Showtec Phantom 65 Spot: https://www.bax-shop.nl/led-moving-head/showtec-phantom-65-spot-led-movinghead
