---
name: casual-game-feature-designer
description: Design persistent non-core systems for casual games, such as onboarding, inventory, tasks, achievements, collections, progression, unlocks, streaks, rankings, settings, saves, and resource flows. Use when the main problem is a lasting feature rather than the core play loop, a time-limited event, or monetization.
---

# Casual Game Feature Designer

Work from the current project's confirmed systems and terminology. Before drafting, confirm every ambiguity that could change scope, state flow, dependencies, rewards, or expected behavior. Do not invent currencies, rewards, values, fields, or technical structures.

## Define the feature

Describe only the needed dimensions:

- player need and feature objective;
- entry, visibility, unlock, and availability;
- core user flow and system state transitions;
- progress, resource, inventory, reward, reset, or persistence rules;
- enabled, disabled, locked, empty, completed, and exception states;
- dependencies on gameplay, account/save, UI, events, or monetization;
- recovery from interruption, restart, disconnect, duplicate action, or failed grant when relevant;
- acceptance conditions.

Keep player action separate from system judgment, display state from data state, and unlock conditions from reward conditions. Make AND/OR relationships and threshold semantics explicit.

## Scope boundaries

- A prop's effect on the board or puzzle belongs to gameplay design; its inventory, unlock, acquisition, and persistent consumption belong here.
- A permanent streak, achievement, collection, or progression system belongs here.
- A system with a defined opening/closing window or rotating cycle belongs to event design.
- Ads, IAP, offers, subscriptions, price, and monetization frequency belong to monetization design.
- Detailed layout, copy, animation, audio, and haptics belong to UX specification.

## Configuration restraint

Use concrete configuration names only when the user supplies an authoritative schema, table, backend view, or field document. If absent, omit the configuration section when it is optional. If the requirement cannot be made coherent without it, ask for the source rather than creating placeholders.

## Output

Answer simple questions directly. For a formal feature spec, default to: purpose and scope; entry/unlock; states and flow; rules; dependencies; exceptions; acceptance. Avoid adding analytics, engineering design, or speculative future systems unless requested.

