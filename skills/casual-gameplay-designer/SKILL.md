---
name: casual-gameplay-designer
description: Design, explain, or revise the core gameplay of a casual game, including actions, mechanics, level rules, states, solvability, difficulty, win/fail/stuck logic, recovery, and prototype validation. Use when the player-facing play loop is the main subject; do not use for standalone live events or monetization systems.
---

# Casual Gameplay Designer

Design from the target project's existing rules rather than treating it as a blank game. Before writing, read the supplied materials and confirm every ambiguity that could change the mechanic, level result, or implementation. Do not import rules from another game.

## Build a testable system

Define only what the task needs:

- player goal and core experience;
- valid player inputs;
- game state and element states;
- legality and system response;
- feedback, consequence, and next decision;
- initialization and progression;
- win, fail, stuck, restart, recovery, revive, or assist behavior;
- dependencies on level generation, UI, props, or persistent systems.

For each major mechanic, distinguish fixed rules from tunable parameters. Cover normal paths, boundary states, failure/recovery paths, irreversible effects, and plausible exploits. Do not invent parameter values.

When solvability or stuck-state logic matters, define the exact search space and judgment timing. Separate “no legal move now” from “no sequence can lead to completion.” Do not call repeated reversible movement a failure unless the rule defines the explored-state or cycle condition precisely enough to avoid premature prediction.

## Difficulty and prototyping

Explain how complexity is introduced and taught without prescribing unnecessary level content. Identify the smallest playable prototype, the weakest design assumption, observable success/failure signals, and the cheapest disconfirming playtest when validation is requested.

Do not claim fun, retention, or difficulty quality without playtest evidence. Label candidate ideas and untested assumptions.

## Boundary with other skills

Gameplay-changing props belong here: their effect, valid target, legal use, and impact on the level. Inventory, unlock, acquisition, purchase, and persistent consumption history belong to feature or monetization design.

## Output

For a narrow question, answer directly. For a formal design, default to: objective and loop; elements/states; operation and judgment rules; win/fail/stuck/recovery; progression or teaching; dependencies and edge cases; prototype or acceptance focus. Keep rules deterministic and developer-ready without dictating code architecture.

