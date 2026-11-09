# Factions and Colours
## Initial visual palette — v0.1

**Purpose:** Establish readable faction colours for map territories, unit counters and UI accents.

These are proposed starting values, not final historical claims or locked art direction. The palette should be tested against the actual map, fog-of-war treatment, small unit silhouettes and common colour-vision deficiencies.

| Faction | Suggested colour | Hex | Character |
|---|---|---|---|
| United States | Steel blue | `#477DA8` | Cool, industrial blue |
| United Kingdom | Khaki / sand | `#B49A68` | Muted tan |
| Soviet Union | Deep red | `#A9473F` | Strong red, slightly muted |
| Germany | Iron grey | `#626B76` | Neutral dark grey |
| Japan | Ochre | `#C58B43` | Warm amber |
| Italy | Olive | `#71836B` | Muted green |

## Usage principles

- Apply faction identity consistently to territories, counters, badges and dispatch metadata.
- Keep unit silhouettes and their role markings consistent across factions.
- Use colour plus shape, iconography, pattern or insignia; never rely on colour alone.
- Maintain legibility on parchment, dark map surfaces and fog overlays.
- Separate ownership colour from unit condition and interaction state.

## Separate visual channels

Faction colour should not also communicate every other state.

Use distinct visual treatments for:

- **Ownership:** faction palette
- **Selection:** outline, glow or raised treatment
- **Damage / strength:** damage markers or strength pips
- **Entrenchment:** defensive marker
- **Supply:** supply icon or line treatment
- **Fog of war:** desaturated / concealed map treatment
- **Contested control:** explicit contested marker or mixed border treatment

## Asset production recommendation

Create one approved base silhouette for each unit type, then produce faction-specific treatments. This is more scalable and visually consistent than creating unrelated models for every faction.

## Validation checklist

- Test all factions adjacent to one another on the map.
- Check unit readability at actual gameplay size, not only in an asset sheet.
- Check contrast under fog of war and night / low-light map treatments.
- Include a colour-blindness review.
- Ensure selected, damaged and supplied states remain distinguishable from faction identity.
