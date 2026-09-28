---
name: casual-game-acceptance
description: Turn casual-game requirements into concise, executable acceptance cases with minimal repetition and backtracking. Use for feature acceptance, regression focus, boundary verification, configuration priority checks, and Debug-assisted construction of hard-to-reach states; do not decide missing product rules on the designer's behalf.
---

# Casual Game Acceptance

Derive every expected result from the current authoritative requirement. Before writing cases, confirm ambiguities that could change the expected outcome, test state, or scope. If the requirement cannot determine the expected result, report the requirement gap and wait rather than inventing behavior.

## Design the smallest complete path

- Prefer one continuous operation sequence that covers several checkpoints.
- Reuse state when safe; split cases only when state isolation is necessary.
- Avoid repeated setup, unnecessary navigation, and backtracking.
- Cover the main flow plus only material failure, exception, boundary, state-transition, restart/reconnect/cross-day, switch, or priority paths.
- Distinguish states reproducible through normal play from states requiring Debug injection or controlled data.
- Use Debug construction when a valid combination is impractical or non-deterministic to reach, and state exactly what condition must be injected without inventing tool fields.
- Do not maximize case count. Optimize for complete, observable, executable coverage.

## Default format

Use this table unless another format is requested:

| 编号 | 前置条件 | 操作步骤 | 预期结果 |
|---|---|---|---|

Add boundary/exception, configuration condition, Debug construction, or unresolved requirement sections only when needed. Keep steps imperative and expected results observable. Do not use rigid Given/When/Then wording if a short operation sequence is clearer.

## Coverage judgment

Check relevant state partitions and boundary values, not every permutation. For multi-factor rules, cover each distinct outcome and priority branch. Flag logical impossibility separately from “hard to reproduce.” If the user asks for a simple case, return the minimum complete set rather than a full QA test library.

