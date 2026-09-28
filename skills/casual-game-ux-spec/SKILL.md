---
name: casual-game-ux-spec
description: Specify casual-game UI, interaction, game copy, animation, visual feedback, audio, and haptics. Use for page structure, component states, click/drag flows, popups, prompts, presentation timing, and player feedback; do not silently redefine upstream gameplay or feature rules.
---

# Casual Game UX Specification

Translate confirmed gameplay and feature rules into what the player sees, does, and receives as feedback. Before writing, confirm any ambiguity that changes state, interaction, timing, copy context, or asset expectation. If an upstream rule is missing or contradictory, report it instead of choosing a new rule.

## Specify the experience

Use only relevant items:

- page purpose, entry, exit, and information priority;
- regions, components, persistent and temporary elements;
- tap, drag, hold, back, close, skip, interrupt, and resume behavior;
- default, selected, locked, disabled, loading, empty, success, failure, and exceptional states;
- popup trigger, content, buttons, close/cancel behavior, and resulting state;
- operation feedback, timing, blocking/non-blocking behavior, and repeated input;
- animation, effects, audio, and haptic trigger, intensity, duration, and interruption when these matter;
- safe area, resolution, overlap, readability, and accessibility risks when relevant;
- dependencies on gameplay, features, art, localization, and implementation.

Prioritize strong haptics for high-confidence, high-value moments such as decisive success or impactful action; use lighter feedback for ordinary confirmation; omit vibration where repetition would fatigue or confuse. Distinguish must-have feedback from optional polish when the user asks for prioritization.

## Copy

Judge copy in its exact trigger and player state. Default to concise Chinese planning text. For English in-game copy, give one natural casual-game primary version plus a Chinese back-translation; add alternatives only when meaningful tone choices exist. Do not polish a sentence in isolation when the issue is actually the underlying rule or scene.

## Output

Answer simple copy or feedback questions directly. For a formal UX spec, default to: page/scene purpose; components and states; interaction flow; popups/prompts; feedback and presentation; exceptions and dependencies. Avoid re-explaining entire upstream systems.

