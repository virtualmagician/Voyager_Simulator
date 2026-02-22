# Voyager Spacecraft Trajectory Simulator

An interactive 3D simulator tracking the Voyager missions from their 1977 launches through planetary encounters to interstellar space in 2026.

## Features

- **Dual Spacecraft** - Both Voyager 1 and Voyager 2 with independent trajectories
- **High-Quality 3D Model** - NASA's official Voyager GLB model embedded directly
- **Journey Mode** - Cinematic guided tour following Voyager through the entire mission
- **Accurate Solar System** - All 8 planets with Keplerian orbital mechanics
- **Complete Grand Tour** - Jupiter, Saturn, Uranus, and Neptune encounters
- **Mission-Accurate Moon Data** - Distinguishes between moons imaged vs discovered
- **Event Popups** - Rich overlays for each major mission milestone
- **Pale Blue Dot** - The iconic 1990 moment when Voyager 1 photographed Earth
- **Interactive Timeline** - Skip between mission events or scrub through 49 years
- **Multiple Camera Views** - Free orbit, follow Voyager, top view, side view
- **Toggleable Overlays** - Show/hide orbits, labels, trajectory trails, spacecraft

## Visual Enhancements

- **Multi-layered Starfield** - Dense background stars with varied colors (white, blue-white, yellow, red)
- **Bright Prominent Stars** - Scattered larger stars for depth
- **Nebula Dust Clouds** - Subtle purple/blue atmospheric dust
- **Enhanced Sun** - Multi-layered corona with yellow, orange, and red glow effects
- **Planet Atmospheres** - Gas giants have subtle atmospheric halos
- **Saturn's Rings** - Detailed rings with Cassini division
- **Uranus Rings** - Faint ring system at proper tilt
- **Glowing Trajectory Lines** - Main lines with subtle glow trails

## Journey Mode

Click the **Journey Mode** button (at the end of the timeline) to experience a guided cinematic journey:

1. **Smooth zoom-in** - Camera arcs around (not through) the sun to approach Voyager
2. **Close follow** - Camera stays locked on Voyager 2 throughout the mission
3. **50× speed** - Fast enough to see the journey, slow enough to appreciate it
4. **Automatic popups** - Each flyby triggers an informational overlay
5. **Dynamic positioning** - Camera stays behind Voyager, looking toward destinations
6. **Toggle off** - Click the button again to exit Journey Mode

The button turns red when active. The tour pauses at each major event. Click "Continue Journey" to resume.

## Mission Timelines

### Voyager 2 - The Grand Tour

| Date | Event | Highlights |
|------|-------|------------|
| August 20, 1977 | **Launch** | Cape Canaveral, beginning the Grand Tour |
| July 9, 1979 | **Jupiter Flyby** | Io volcanism, Europa ice, ring system discovered |
| August 26, 1981 | **Saturn Flyby** | Titan atmosphere, complex ring structure |
| January 24, 1986 | **Uranus Flyby** | First visit! 10 new moons, Miranda's cliffs |
| August 25, 1989 | **Neptune Flyby** | First visit! Triton geysers, 6 new moons |
| August 30, 2007 | **Heliosheath Entry** | Crossed termination shock at 84 AU |
| November 5, 2018 | **Interstellar Space** | Crossed heliopause at 119 AU |

### Voyager 1 - Fastest & Farthest

| Date | Event | Highlights |
|------|-------|------------|
| September 5, 1977 | **Launch** | Faster trajectory than Voyager 2 |
| March 5, 1979 | **Jupiter Flyby** | First to image Io's volcanoes |
| November 12, 1980 | **Saturn Flyby** | Titan flyby ended Grand Tour option |
| February 14, 1990 | **Pale Blue Dot** | Earth photographed from 6 billion km |
| December 16, 2004 | **Heliosheath Entry** | First to reach heliosheath at 94 AU |
| August 25, 2012 | **Interstellar Space** | First human-made object in interstellar space |

## Moons - Imaged vs Discovered

### Jupiter System
- **Imaged:** Io, Europa, Ganymede, Callisto, Amalthea
- **Discovered:** Thebe, Metis

### Saturn System  
- **Imaged:** Titan, Mimas, Enceladus, Tethys, Dione, Rhea, Hyperion, Iapetus, Phoebe
- **Discovered (V1):** Atlas, Prometheus, Pandora

### Uranus System (Voyager 2 only)
- **Imaged:** Miranda, Ariel, Umbriel, Titania, Oberon
- **Discovered:** Puck, Juliet, Portia, Rosalind, Desdemona, Bianca, Ophelia, Cordelia, Cressida, Perdita

### Neptune System (Voyager 2 only)
- **Imaged:** Triton, Nereid
- **Discovered:** Proteus, Larissa, Despina, Galatea, Thalassa, Naiad

## Controls

### Mouse
- **Drag** - Rotate camera
- **Scroll** - Zoom in/out

### Keyboard
- **Space** - Play/Pause timeline
- **H** - Toggle UI visibility
- **L** - Toggle labels
- **O** - Toggle orbital paths
- **T** - Toggle trajectory trail

### Timeline Controls
- **Journey Mode** - Start/stop guided cinematic tour (red when active)
- **▶ / ⏸** - Play/Pause timeline
- **⏮ / ⏭** - Skip to previous/next mission event (with popup)
- **1× / 10× / 100× / 1000×** - Playback speed
- **Click timeline markers** - Jump directly to events

### Toggle Buttons
- **Voyager 1 / Voyager 2** - Show/hide each spacecraft
- **Orbits** - Planetary orbital paths
- **Labels** - Planet and spacecraft names
- **Trail** - Trajectory path visualization

## Usage

The simulator can be opened directly in a browser - no server required. The 3D model is embedded in the HTML file.

Simply open `index.html` in your browser.

Alternatively, you can run a local server:

```bash
cd simulator
python3 -m http.server 8080
open http://localhost:8080
```

## Technical Details

- Built with Three.js (WebGL)
- Single-file HTML application (~3200 lines)
- Embedded NASA Voyager GLB model (base64 encoded)
- Swiss red accent color (#DA291C)
- No build process required
- Uses CDN for Three.js library
- Bezier curve camera paths for smooth cinematic movement
- Multi-layer visual effects for stars, sun, and planets

## Data Sources

- Trajectory data based on NASA JPL Voyager mission data
- Planetary orbital elements from NASA Solar System Dynamics
- Mission timeline from NASA JPL Voyager Mission page
- Moon discoveries verified against NASA Science documentation

## Credits

- Marco Tempest, ETH Zurich | Space
- Voyager 3D model from NASA's official GLB model
- Quote by Carl Sagan (Pale Blue Dot)

---

*Voyager 1 is the most distant human-made object at over 165 AU from the Sun.*
*Voyager 2 is the only spacecraft to have visited all four gas giant planets.*
