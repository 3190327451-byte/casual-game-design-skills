# Casual Game Design Skills

A project-neutral Codex skill suite for casual, puzzle, hyper-casual, hybrid-casual, light simulation, idle, decorating, and collection games.

## Included skills

- `game-design-doc-writer`: umbrella router for broad or cross-domain requests.
- `casual-game-research`: game, competitor, genre, and lightweight opportunity research.
- `casual-gameplay-designer`: core mechanics, level rules, solvability, and failure/recovery design.
- `casual-game-feature-designer`: persistent non-core feature and system design.
- `casual-game-event-designer`: time-limited and rotating event design.
- `casual-game-monetization-designer`: ads, IAP, offers, subscriptions, and monetization review.
- `casual-game-ux-spec`: UI, interaction, copy, animation, audio, and haptic specification.
- `casual-game-doc-reviewer`: single-document, cross-document, current-state, and change-impact review.
- `casual-game-acceptance`: concise, executable acceptance cases with minimal repetition.

## Design principles

- Confirm material ambiguities before starting work.
- Treat supplied project sources as authoritative and do not carry project-specific rules into another game.
- Identify conflicts and consequences before adopting a newly confirmed rule.
- Never invent configuration fields, values, currencies, rewards, or project facts.
- Default to concise, actionable output and edit external documents only when explicitly requested.

## Installation

Copy the desired folders from `skills/` into your Codex skills directory:

```text
~/.codex/skills/
```

The umbrella router and all specialist skills support implicit invocation. Each specialist can also be invoked explicitly by its skill name.
