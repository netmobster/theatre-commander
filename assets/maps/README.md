# Map Assets

## Europe Map Alpha

- **Asset name:** Europe Map Alpha
- **Status:** Visual direction reference; not production map data
- **Intended location:** `assets/maps/europe-map-alpha.jpg`
- **Source artwork:** ChatGPT-generated concept image, 1536 × 1024
- **Visual direction:** Neutral grey land territories; vivid deep-blue oceans; bright sea-zone boundaries; high-contrast territory borders and labels.

### Intended use

This artwork establishes the visual direction for the first Europe theatre map. It is a presentation reference only.

The production map must be rebuilt as independently addressable territory geometry (preferably SVG paths or equivalent vector data) with stable territory IDs. Ownership colour, selection, combat highlights, and fog of war must be separate render layers. Do not treat the flattened concept artwork as authoritative territory geometry or adjacency data.

### Ownership colour principle

Land territories begin neutral grey. On capture, the territory fill is tinted with the owning faction's palette. Ocean, sea-zone boundaries, labels, coastlines, and interface overlays remain independent of territory ownership.

### Source file

The generated source image is available in the originating ChatGPT conversation as `a_detailed_polished_map_illustration_a_theatre.png`. The binary image itself has not yet been transferred into this repository; this file records its intended asset path and implementation notes.
