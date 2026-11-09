# Unit Asset Specification
## Initial production brief — v0.1

## Goal

Create a cohesive visual language for the baseline land, air and naval units in the unit catalogue. Each unit should be identifiable by silhouette at normal gameplay scale and remain legible over a detailed strategic map.

## Asset family strategy

Use a shared base silhouette per unit type, then create faction-specific visual treatments through:

- Faction colour
- Historically inspired insignia or markings, used consistently and tastefully
- Small equipment or detailing differences where they improve recognition
- Optional faction-specific variations only when the silhouette remains instantly readable

Avoid creating six completely unrelated designs for the same unit role.

## Required initial units

### Land
- Infantry
- Artillery
- Mechanized infantry
- Tank / armour
- Anti-aircraft artillery

### Air
- Fighter
- Tactical bomber
- Strategic bomber

### Naval
- Transport
- Submarine
- Destroyer
- Cruiser
- Battleship
- Aircraft carrier

### Infrastructure
- Industrial complex
- Airbase
- Naval base

## Presentation variants

Each unit asset should be designed to support:

1. Map-scale representation
2. Selected / highlighted state
3. Damaged or reduced-strength state
4. Entrenched / fortified state where applicable
5. Tooltip or inspection close-up

## Visual direction

- Strong, legible silhouettes
- Period-inspired material and equipment language
- Slightly stylized for clarity rather than photorealistic miniatures
- Consistent camera angle, lighting and scale within each asset family
- Restrained faction-specific colour application
- Avoid tiny detail that disappears at map scale

## Technical requirements to decide

These are intentionally not locked yet:

- 2D counters, 2.5D miniatures or 3D models
- Orthographic camera angle and rotation rules
- Native asset resolution and export sizes
- Transparent backgrounds versus baked map shadows
- Animation requirements for movement and combat
- Whether naval and air units share the same map-scale treatment as land units
- Required sprite atlas or individual-file conventions

## First production milestone

Produce a small proof sheet before building the full catalogue:

- Infantry
- Tank
- Fighter
- Battleship

Render each in all six proposed faction colours. Review readability, visual consistency and colour differentiation at realistic gameplay scale before expanding the set.
