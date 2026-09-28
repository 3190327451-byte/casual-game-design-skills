---
name: game-design-doc-writer
description: Route broad or ambiguous casual-game planning requests to the right specialist workflow, coordinate multi-domain design work, and draft or revise game design documents when the request spans gameplay, features, events, monetization, UX, review, or acceptance. Use this umbrella skill when the user has not named a clearer specialist task or asks for one integrated deliverable.
---

# Casual Game Design Router

Use this skill as the project-neutral entry point for casual, hyper-casual, hybrid-casual, puzzle, light simulation, idle, decorating, and collection games. Do not carry mechanics, fields, values, or terminology from one game into another.

## Before starting

Read the supplied project materials and establish the current design baseline. Before producing the deliverable, ask about every ambiguity that could change the content, logic, scope, authority, or output. Ask one decisive question at a time when practical, and begin only after the material uncertainties are resolved. Do not ask about harmless formatting details; preserve the source style.

Use this source priority:

1. the baseline document or rule explicitly designated for the current task;
2. the project's latest valid documents and live configuration;
3. a new rule confirmed by the user in the conversation;
4. historical documents or reference games;
5. general design practice.

A user reply such as “可以” or “OK” confirms the proposed rule. Before treating a new rule as authoritative, identify what old rule it conflicts with, the resulting player/development/configuration/acceptance impact, and the documents that must change. Do not silently overwrite conflicts.

## Route the request

Use the named specialist directly when the request is clear:

- game/competitor/market research: `casual-game-research`;
- core mechanics, level rules, solvability, win/fail: `casual-gameplay-designer`;
- persistent non-core systems: `casual-game-feature-designer`;
- timed or rotating activities: `casual-game-event-designer`;
- ads, IAP, offers, subscriptions, and monetization configuration: `casual-game-monetization-designer`;
- UI states, interaction, copy, animation, audio, and haptics: `casual-game-ux-spec`;
- document logic review, cross-document consistency, or change impact: `casual-game-doc-reviewer`;
- acceptance cases and requirement verification: `casual-game-acceptance`.

For a compound request, choose one primary workflow and add only the specialist checks required to complete it. Share one project baseline, avoid repeated questions, and return one integrated result. Do not expose internal routing unless it helps the user.

## Shared constraints

- Distinguish documented facts, verified observations, reasonable inference, proposals, and unverified assumptions.
- Do not invent project facts, values, rewards, currencies, fields, data structures, or configuration names.
- If concrete configuration is required but no authoritative schema was supplied, omit that section when optional; when essential, stop and ask for the schema.
- Keep core rules in one authoritative location and reference them elsewhere instead of rewriting them inconsistently.
- Default to concise Chinese, conclusion first. Match the requested format and expand only when needed.
- For English in-game copy, provide one natural primary version and a Chinese back-translation unless the user asks otherwise.
- Do not edit Feishu, local files, or other external documents unless the user explicitly asks for the write. When editing is authorized, preserve structure and make the minimum necessary change.
- Exclude gambling, heavy RPG, MMO, and complex SLG work unless the user explicitly expands the scope.

## Delivering work

Answer a narrow question directly rather than forcing a full template. For a formal document, choose the smallest structure that makes rules, states, dependencies, edge cases, and acceptance observable. Never add analytics, technical implementation, art lists, or configuration sections merely for completeness.

