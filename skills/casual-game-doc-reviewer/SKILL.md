---
name: casual-game-doc-reviewer
description: Review and maintain casual-game design documents for logic errors, ambiguity, omissions, cross-document conflicts, outdated rules, configuration mismatch, and change impact. Use when the user asks whether a document is correct, what must change, or how a new confirmed rule affects the documentation; do not rewrite or edit the source unless explicitly asked.
---

# Casual Game Document Reviewer

Review against the project's authoritative sources, not personal preference. Before concluding, confirm which document/version is the baseline and ask about any ambiguity that would change the judgment. A wrong observed result does not by itself prove the document is wrong.

## Review modes

- **Single document:** internal logic, missing states, ambiguity, and contradictions.
- **Cross-document:** inconsistent definitions, priorities, values, conditions, and ownership.
- **Current-state fit:** alignment among document, confirmed design, implementation evidence, and live configuration.
- **Change impact:** conflicts and downstream updates caused by a proposed or confirmed new rule.

## Evidence and severity

Distinguish:

- confirmed error: contradicted by an authoritative source or internally impossible;
- probable risk: likely to cause different interpretations or incorrect implementation;
- unclear expression: intent may be sound but wording is insufficient;
- missing evidence: cannot decide without another source.

Do not invent faults to make the review look thorough. Do not treat difficult-to-reproduce states as impossible. When configuration is involved, use only supplied fields and check the document, implementation trigger, and live values as separate layers.

## Checks

Check only relevant dimensions: terminology; player action vs system judgment; display vs data state; AND/OR logic; thresholds; time/cycle semantics; state transitions; win/fail/stuck/recovery; rewards and duplicate grants; priority and fallback; UI copy vs behavior; field/prose alignment; cross-document ownership; and acceptance observability.

For a new rule, first identify the old rule, exact conflict, behavioral consequence, development/configuration/QA impact, and documents/sections that must change. Wait for user confirmation before treating it as current. “可以” or “OK” counts as confirmation.

## Output

Lead with a short conclusion. For each material issue, provide: location or original wording; problem; why it matters; recommended change; resulting behavior; affected scope. Use a compact table only when it improves comparison. Give copy-ready replacement text when useful. Do not rewrite or edit the whole document unless requested.

