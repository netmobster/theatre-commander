# Theatre Commander
## Game Concept — v0.2
**Captured:** 9 November 2026  
**Status:** Early concept; mechanics intentionally open

## Premise

A global Axis & Allies-inspired war game in which the player is always the **Commander-in-Chief**, but can directly command only **one theatre at a time**.

The player chooses where to be operationally present. In that theatre, they play a focused strategy game built around territory control, income, production, unit composition, movement and combat.

Everywhere else, the war continues under persistent AI theatre generals. The Commander-in-Chief receives dispatches, issues orders, allocates resources and lives with the consequences.

**You are responsible for the whole war, but cannot personally be everywhere.**

## One game, one role

There are no separate Commander-in-Chief and General game modes. The player is always Commander-in-Chief.

At the start of each turn, the player may choose which theatre to inhabit, for example:

- Europe
- Africa
- Pacific

The active theatre is played directly. All other theatres are commanded indirectly through generals and dispatches.

This is a deliberate constraint: the player gets the full strategic texture of Axis & Allies within a manageable theatre, while the wider war remains alive.

## Active theatre: direct command

The active theatre should retain the familiar pleasures and decisions of an Axis & Allies-style game:

- Territories, ownership and income
- Purchasing and producing units
- Unit placement and reinforcement
- Movement and combat
- Land, sea and air power
- Strategic positioning, chokepoints and supply
- Capturing, defending and consolidating territory

The theatre must feel like a complete, meaningful strategy game—not a cut-down map or a simplified minigame.

## Inactive theatres: dispatch command

Outside the active theatre, the player cannot directly manipulate units or freely inspect the full operational map. They interact through their subordinate generals.

Dispatches include situation reports, requests, warnings, recommendations, claims of progress and reports of failure.

The player responds with direction: hold, advance, prepare an offensive, exploit a breakthrough, conserve forces, prioritize an objective, request or release resources, reinforce, withdraw, or change a standing mission.

Orders express intent and constraints. They should not become remote unit-by-unit clicking.

## The dispatch cycle

1. Reports arrive from inactive theatres.
2. The Commander-in-Chief assesses competing needs, risks and opportunities.
3. The player issues orders, changes priorities and allocates resources.
4. At the start of the turn, the player chooses the theatre to inhabit.
5. The turn resolves: the player directly commands the active theatre while AI generals operate the others.
6. New dispatches report what happened.

The player acts on reports, then discovers the consequences after the turn resolves. They do not continuously watch every theatre play out.

## Generals: persistent commanders, not scripts

Each inactive theatre has a general who continues to command it over time.

A general has:

- Persistent identity and personality
- Military doctrine and preferred approach
- Competence and judgment
- Current assignment or standing mission
- Forces, resources and local responsibilities
- An operational picture based on available information
- Defined authority and constraints
- A history of orders, decisions and outcomes

A general has an ongoing job, not merely an optimization goal. They continue working until the assignment is completed, changed or made irrelevant.

On completion, they may consolidate, fortify, replenish, accumulate resources, prepare a new operation or request further orders.

Generals should exercise genuine judgment. They may make decisions the player would not have made.

When the player leaves a theatre, its general inherits the current operational situation. When the player returns, they find the consequences of that general's command.

## Reports, uncertainty and trust

Dispatches are a core game mechanic, not flavour text.

Reports can be incomplete, delayed, mistaken or misleading for grounded reasons:

- **Fog of war:** the general does not know what the enemy is doing.
- **Delay:** information is accurate but no longer current.
- **Assessment error:** the general misreads the situation.
- **Personality:** optimism, pessimism, caution or overconfidence shape interpretation.
- **Competence:** generals differ in their ability to assess risk and outcomes.
- **Self-preservation:** a general may minimize or conceal failures.
- **Interpretation or disobedience:** a general may depart from the literal order because they believe another course is necessary.

Reports must not be randomly unreliable. Reliability emerges from the general, the information available and the circumstances. A capable general can be wrong; a dishonest general can sometimes tell the truth.

Reconnaissance and independent intelligence channels may later give the player ways to improve confidence.

## Attention is a strategic resource

The player has global responsibility but only one active theatre.

Choosing where to be present is itself a consequential decision. Europe may have a breakthrough opportunity while the Pacific faces a fleet threat and Africa is short of supply. The player must decide where direct attention matters most.

The challenge is deciding what deserves personal attention, what can be delegated and which generals can be trusted.

## Multiplayer

The same command structure supports multiplayer.

Human players can each be Commander-in-Chief of a country or side, with AI generals operating inactive theatres. Each player receives dispatches from their own command structure and directs their own forces.

One possible configuration is four human Commanders-in-Chief, each with four AI subordinate generals: four humans and sixteen AI theatre commanders. Exact numbers and theatre assignments remain scenario-dependent.

Players compete globally while experiencing the war through limited operational perspectives. They do not receive omniscient access to opposing command structures.

Shared human command of one country is a possible extension, not a settled requirement.

## Architectural reference: Elsewhere's intent-to-reality model

Theatre Commander can build on the interaction pattern explored in **Elsewhere**:

**Intent → AI interpretation → authoritative simulation → consequence → persistent context → next intent.**

In Elsewhere, the player expresses intent rather than prescribing every mechanical action. AI interprets it, the engine determines what actually happens, consequences persist, and the changed world informs the next interaction.

Theatre Commander applies this to military command:

| Elsewhere | Theatre Commander |
|---|---|
| Player expresses intent | Commander issues a dispatch |
| AI interprets intent | General interprets orders |
| Engine resolves reality | War simulation resolves operations |
| Consequences persist | Territory, casualties, resources and positions change |
| Player discovers what happened | Commander receives a front dispatch |
| Player expresses new intent | Commander issues revised orders |

### AI does not define reality

A general may interpret orders, assess a situation, propose an operation and make decisions within its authority. The authoritative war simulation determines what actually happens.

A general cannot narrate a victory into existence. It commits decisions to the simulation; the simulation resolves them according to the rules. The general then reports the outcome based on what it knows, including uncertainty, error, bias or deliberate misrepresentation.

The pattern carried over from Elsewhere is natural intent, bounded AI authority, authoritative world state, persistent consequences and context-aware continuation.

Theatre Commander adds military doctrine, command authority, standing missions, resource allocation, turn-based resolution, intelligence and reporting.

**Elsewhere is a world you influence through intent. Theatre Commander is a war you lead through intent.**

This is an architectural reference, not a claim that the games share an implementation or simulation rules.

## Explicit scope constraint: no diplomacy

**There is no diplomacy system.**

The player is commanding a war, not running a foreign ministry. Do not add diplomatic negotiation, relationship meters, treaty management or a diplomacy minigame.

Other nations remain part of the simulation. Their forces, territories, production, movements and decisions matter. The player's strategic interaction is through military command.

The strategic layer focuses on:

- Military objectives and theatre priorities
- Resource allocation, production and reinforcement
- Orders to subordinate generals
- Intelligence and reconnaissance
- Operational decisions
- Reports, uncertainty and accountability

**Complexity should come from military decisions and imperfect information, not from accumulating management systems.**

## Design principles

1. Preserve the Axis & Allies-style strategic economy, territory control, production, unit decisions and combat.
2. Restrain the playable scope to a meaningful theatre.
3. Keep the wider war alive while the player is elsewhere.
4. Make delegation consequential through persistent generals with judgment and limitations.
5. Use dispatches as the interface to the wider war.
6. Make information imperfect but fair.
7. Make attention a resource.
8. Keep the simulation authoritative; AI interprets and decides within the rules.
9. Do not add diplomacy.

## Open design questions

- What exactly constitutes a theatre, and how do boundaries vary by scenario?
- How are global production, income and resources divided between theatres?
- What authority does a general have to interpret, delay or refuse an order?
- How much information does the Commander-in-Chief receive about inactive theatres?
- How are intelligence and report reliability communicated?
- What does the outgoing general inherit when the player switches theatres?
- Can multiple humans share one command structure?
- How many subordinate generals suit a scenario?
- Is turn resolution simultaneous, sequential or theatre-specific?

## One-sentence pitch

**An Axis & Allies-inspired global war game where you are always Commander-in-Chief, but can only personally command one theatre per turn; everywhere else, your generals fight the war, and you lead them through dispatches.**
