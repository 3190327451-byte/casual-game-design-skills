---
name: casual-game-event-designer
description: Design time-limited, rotating, seasonal, competitive, cooperative, or milestone events for casual games. Use for event loops, participation, progress, rewards, timing, settlement, reset, ranking, and event edge cases; do not use as the primary workflow for permanent features or standalone ad/IAP rules.
---

# Casual Game Event Designer

Base the event on the target project's confirmed gameplay, resources, and persistent systems. Before drafting, confirm unclear objectives, timing semantics, eligibility, progress source, reward source, and settlement behavior. Do not create missing currencies, rewards, values, or configuration fields.

## Define the event loop

Cover only what is relevant:

- event objective and intended player behavior;
- opening, closing, unlock, entry visibility, and eligibility;
- the action that creates event progress and when it is counted;
- stages, tasks, event resources, personal/cooperative/competitive progress;
- reward preview, generation, grant, claim, duplicate prevention, and unclaimed handling;
- cycle, local/server time basis, cross-day behavior, refresh, reset, settlement, and expiry;
- ranking, tie, promotion/demotion, or group logic when applicable;
- interaction with base gameplay and persistent features;
- interruption, offline, reconnect, version update, late entry, missing reward, and disabled-event states when relevant.

Separate calendar labels, cycle day, accumulated count, and displayed progress. Make AND/OR conditions and threshold boundaries explicit.

## Boundary with monetization

An event may state when it calls an ad, offer, or purchase entry and what event result follows. The monetization workflow owns ad eligibility, frequency, inventory, price, purchase validation, and failure policy. Reference those rules instead of duplicating them.

## Metrics and claims

State expected directional effects on participation, completion, return, or retention only as hypotheses unless supported by data. Include the smallest useful validation signal when the user asks about impact.

## Output

For a formal event spec, default to: positioning; timing/unlock/entry; event loop; progress and rewards; settlement/reset; integrations; edge cases; acceptance. Omit unused sections and keep one authoritative definition for each rule.

