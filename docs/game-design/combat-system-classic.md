# Classic Combat System

**Status:** Historical baseline  
**Version:** 1.0  
**Rules reference:** Original Axis & Allies Classic (1980s-era ruleset; use the Classic / second-edition rules as the working reference)

This document records the combat values and defining combat rules to preserve from the Classic game. It is a baseline for Theatre Commander, not a commitment to reproduce every physical-board procedure unchanged. Any modernization should be explicit and documented as a Theatre Commander rule.

## 1. Core combat model

- Combat uses six-sided dice (D6).
- Each participating unit rolls one die.
- The unit's attack or defence value is its hit threshold.
- A roll equal to or lower than the relevant value scores a hit.
- A value of 0 means the unit does not roll to score hits in that role.
- Attack and defence values are different; use the appropriate value for the side currently rolling.

Combat is resolved in rounds. The attacker rolls, the defender assigns casualties, and the defender returns fire. Casualties assigned in a round still get to return fire in that round. The exchange is therefore simultaneous for casualty purposes, rather than allowing the first side to remove opposing units before they can shoot.

## 2. Classic unit combat values

| Unit | Attack | Defence | Movement |
|---|---:|---:|---:|
| Infantry | 1 | 2 | 1 |
| Armour (tank) | 3 | 2 | 2 |
| Anti-aircraft gun | Special | Special | 1 |
| Fighter | 3 | 4 | 4 |
| Bomber | 4 | 1 | 6 |
| Aircraft carrier | 1 | 3 | 2 |
| Battleship | 4 | 4 | 2 |
| Submarine | 2 | 2 | 2 |
| Transport | 0 | 1 | 2 |
| Industrial complex | — | — | 0 |

**Movement** is the Classic unit movement allowance, not a combat bonus. Air movement is subject to the requirement to reach a valid landing space at the end of the move. Naval units have their Classic sea-zone movement limits.

## 3. Special rules

### Anti-aircraft guns

- AA guns do not make ordinary land-combat attack or defence rolls.
- When enemy aircraft fly over a territory containing an AA gun, the gun fires once at each enemy aircraft.
- Each AA shot hits only on a roll of 1.
- Aircraft hit by AA fire are removed; there is no ordinary return fire against the gun for these shots.
- The Classic rules limit the number of AA guns that can operate in a territory; additional captured or moved guns do not stack additional shots.
- An AA gun is captured with its territory rather than destroyed merely because ownership changes.

### Armour

- Armour attacks at 3 and defends at 2.
- Armour moves two spaces.
- Classic blitz movement allows armour to pass through an enemy-controlled but unoccupied territory, capturing it and continuing its move, subject to the original movement and territory restrictions.

### Fighters

- Fighters attack at 3 and defend at 4.
- Fighters move up to four spaces.
- Fighters can participate in land and sea combat.
- At sea, fighters require a friendly aircraft carrier on which to land. A Classic carrier can accommodate up to two fighters.

### Bombers

- Bombers attack at 4 and defend at 1.
- Bombers move up to six spaces.
- Bombers can conduct strategic bombing raids against industrial complexes.
- In a strategic bombing raid, surviving bombers roll for damage; the resulting damage is deducted from the defender's IPCs, subject to the Classic raid and anti-aircraft procedures.

### Battleships

- Battleships attack and defend at 4.
- Battleships move up to two sea zones.
- During an amphibious assault, a battleship can provide a one-time shore bombardment before the land battle. Each eligible battleship fires one die at its attack value.
- Shore bombardment is separate from the normal naval battle and is not repeated every land-combat round.

### Aircraft carriers

- Carriers attack at 1 and defend at 3.
- Carriers move up to two sea zones.
- A carrier can carry up to two friendly fighters. Carrier-based fighters must have a valid landing carrier at the end of their movement.

### Submarines

- Submarines attack and defend at 2.
- Submarines move up to two sea zones.
- Submarines have a special opening-fire rule in naval combat: they fire before the normal exchange, and units hit by this opening strike do not return fire against that strike.
- Their ability to submerge or withdraw follows the Classic submarine-specific restrictions; do not generalize ordinary retreat rules to submarines.

### Transports

- Transports have no attack roll and defend at 1.
- Transports move up to two sea zones.
- A transport carries either one tank, one AA gun, or up to two infantry, within the Classic loading and unloading rules.
- Cargo does not participate in naval combat while aboard the transport.

### Industrial complexes

- Industrial complexes do not attack, defend, or move.
- They are production infrastructure, not combat units.
- Classic production capacity is governed by the rules for the territory and the industrial complex; newly constructed complexes have the Classic territory-income production limitation.

## 4. Combat procedure: design baseline

For Theatre Commander, preserve these core properties unless a deliberate modernization is recorded:

1. **Unit-specific thresholds.** Each unit type has its own attack and defence values.
2. **D6 resolution.** No separate hit-point or damage-roll system is implied by the basic combat table.
3. **Round-based exchange.** Both sides get their round's fire, including units assigned as casualties in that exchange.
4. **Defender casualty choice.** The defender chooses which units are lost from hits, within the Classic casualty rules.
5. **Special-case procedures stay special.** AA fire, submarine opening fire, strategic bombing, and battleship shore bombardment are distinct procedures, not generic modifiers applied to every battle.
6. **No invented unit classes.** This baseline applies to the ten unit types in the Classic unit catalogue.

## 5. Scope and edition note

The values above are the working reference for the 1980s Classic ruleset, specifically the Classic / second-edition rules used as the baseline in this project. Axis & Allies has multiple printings and editions; do not silently mix in later-edition unit types, combat values, damage rules, or special abilities.

This is a historical rules reference, not a final implementation specification. Where a physical-board procedure needs adaptation for digital play, record the Theatre Commander interpretation separately so the distinction between **Classic rule** and **Theatre Commander modernization** remains visible.

## 6. Related project documents

- `docs/game-design/unit-catalogue.md` — approved Classic unit roster.
- `docs/game-design/factions-and-colours.md` — approved faction colour palette.
- `docs/concept/game-concept.md` — overall game and command-layer concept.
