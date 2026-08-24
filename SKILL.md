---
name: fm26-scout-player-analyst
description: Analyze FM26 player screenshots from FM Scout Engine/FMST26 or similar scouting views, then give grounded player evaluation, tactical fit, role, position, and individual training advice. Use when the user provides Football Manager 2026 player attributes, screenshots, or scouting-tool data and asks whether/how to use the player.
---

# FM26 Scout Player Analyst

Use this skill when the user wants a Football Manager 2026 player judged from a screenshot or copied scouting data, especially FM Scout Engine/FMST26 player pages, attribute grids, role panels, radar charts, percentile tables, or hidden-attribute views.

## First Read

Before analyzing a player, read [references/analysis-guide.md](references/analysis-guide.md). It contains the source hierarchy, screenshot extraction rules, FM26-specific tactical assumptions, evaluation rubric, and output template.

## Operating Rules

- Treat the screenshot as the primary evidence. Extract only visible values, and mark uncertain or cropped values as uncertain instead of guessing.
- Ground advice in FM26's phase split: assess In Possession and Out of Possession role fit separately when enough information is visible.
- Prefer role and position recommendations that fit the player's attribute cluster, age, footedness, physical profile, traits, personality/hidden data if visible, and the user's stated tactic or squad need.
- When the user does not specify a tactic, give recommendations for two or three common tactical contexts instead of pretending there is one universal best role.
- Distinguish game-visible evidence from editor/scouting-tool-only evidence such as CA, PA, hidden attributes, percentile benchmarks, or custom ratings.
- If current FM26 role names, training UI, or community benchmarks matter and are not already present in the task context, verify them against current sources before making precise claims.

## Output Shape

Keep the answer practical and manager-facing:

1. One-line verdict: current level, upside, and best use.
2. Evidence table: strengths, risks, and unknowns from the screenshot.
3. Best positions and IP/OOP role suggestions, with confidence.
4. Tactical fit: systems that amplify the player and systems to avoid.
5. Individual training and traits: one priority plan, not a shopping list.
6. Recruitment/development decision: buy/loan/start/rotate/sell/watch, depending on context.

When the image is unreadable, ask for a clearer screenshot or a copied attribute list, but still summarize what can be safely inferred.
