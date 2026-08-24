# FM26 Player Screenshot Analysis Guide

## Source Hierarchy

Use sources in this order when a claim needs verification:

1. Official Football Manager/Sports Interactive material for FM26 mechanics, role-system changes, training UI, and terminology.
2. FM Scout/FMST26 documentation for how FM Scout Engine-like tools expose attributes, hidden data, percentiles, benchmarks, and profile panels.
3. Established FM community references such as sortitoutsi, FMInside, FM Dossier, and high-quality community guides for role attribute groupings or interpretation.
4. The user's save context and screenshot evidence.

Do not present a community table or tool-derived rating as official match-engine truth. Say "community benchmark", "tool rating", or "visible scouting-tool data" when that is the actual source.

Useful current reference targets:

- Official FM26 tactics article: https://www.footballmanager.com/fm26/features/possession-out-possession-fm26s-new-tactical-evolution
- Official FM26 youth development/training article: https://www.footballmanager.com/the-dugout/top-tips-youth-development-fm26
- FMST26 tool page: https://www.fmscout.com/a-fmst-26.html
- FM Scout player/profile guide: https://www.fmscout.com/player.htm
- FMInside attribute explainer: https://fminside.net/guides/positional-guides/28-player-attributes-in-football-manager
- sortitoutsi FM26 role-attribute guide: https://sortitoutsi.net/content/75078/fm26-important-attributes-for-every-role

## Screenshot Extraction

When given an image, read it like a scout report:

- Identify player name, age, nationality, club, positions, preferred foot, height, value, wage, contract, media description, personality, traits, CA/PA, reputation, and any visible scouting-tool ratings.
- Extract Technical, Mental, Physical, Goalkeeping, Set Pieces, Hidden, and Personality attributes only when visible.
- Preserve 1-20 attribute values exactly. For heatmaps, percentiles, stars, bars, or role scores, state the scale if visible.
- Mark unclear numbers as `unclear`, not as approximate values, unless the user asks for a best-effort read.
- If multiple screenshots show the same field differently, prefer the most recent or highest-resolution image and mention the conflict.

## FM26-Specific Assumptions

FM26 separates In Possession and Out of Possession formations and roles. Roles are no longer judged only through the old single-role plus duty lens. Out of Possession role suitability depends on positional familiarity and key role attributes. The tactical advice should therefore answer:

- What should this player do with the ball?
- What should this player do without the ball?
- Does the transition between those two jobs make physical, mental, and positional sense?

FM26 individual training can include phase role focuses and an additional focus. For younger players, the official guidance emphasizes physical and position development before over-specializing; from roughly 18-21, round technical deficiencies and prime the player for the desired squad role; from 21 onward, refine mental/technical weaknesses and consider suitable traits.

## Evaluation Rubric

Evaluate in layers:

### 1. Attribute Clusters

- Technical execution: First Touch, Passing, Technique, Crossing, Dribbling, Finishing, Long Shots, Marking, Tackling, Heading.
- Mental reliability: Decisions, Anticipation, Concentration, Composure, Teamwork, Work Rate, Positioning, Off the Ball, Vision, Flair.
- Physical platform: Pace, Acceleration, Agility, Balance, Strength, Stamina, Natural Fitness, Jumping Reach.
- Risk indicators: low Decisions/Concentration for central defensive roles, low Work Rate/Teamwork for pressing systems, low Stamina/Natural Fitness for high-volume roles, low Balance/Agility for tight-space attacking roles, low Bravery/Strength/Jumping Reach for aerial or contact-heavy roles.

### 2. Role Fit

For each likely position, score role fit qualitatively:

- `Excellent`: key attributes are strong, weak points are non-critical, and physical/mental profile supports the role.
- `Good`: most key attributes fit, with one or two manageable weaknesses.
- `Conditional`: works only in a specific tactic or with compensating teammates.
- `Developmental`: plausible future role, but not ready now.
- `Avoid`: role asks the player to repeatedly perform against visible weaknesses.

If using community role-attribute tables, use them as a checklist, not as a deterministic calculator.

### 3. Tactical Fit

Recommend contexts that fit the player:

- Pressing/high block: Work Rate, Teamwork, Aggression, Anticipation, Stamina, Pace/Acceleration, Positioning or Off the Ball as relevant.
- Possession/control: First Touch, Passing, Technique, Decisions, Composure, Vision, Teamwork.
- Transition/counter: Pace, Acceleration, Off the Ball, Anticipation, Decisions, Dribbling or Finishing depending on role.
- Low block/direct: Positioning, Concentration, Strength, Jumping Reach, Heading, Work Rate, Passing/Kicking for outlet play.

Mention whether the player needs protection, a runner, a sitter, width, aerial support, or a creative partner.

### 4. Development and Training

Give one primary training plan:

- Role focus: choose IP and OOP role focuses that match the intended pathway.
- Additional focus: choose one weakness with high leverage, such as Quickness, Endurance, Strength, Final Third, Defensive Positioning, Ball Control, Passing, or Chance Conversion.
- Traits: suggest only traits that reinforce the role and current attributes. Avoid traits that magnify a weakness.
- Minutes plan: for prospects, describe match level and loan logic if relevant.

## Response Template

Use Chinese unless the user asks otherwise.

```markdown
**一句话结论**
<当前定位 + 未来上限/风险 + 最推荐用法>

**截图证据**
| 维度 | 看到的内容 | 解读 |
| --- | --- | --- |
| 强项 | ... | ... |
| 短板 | ... | ... |
| 不确定 | ... | ... |

**位置与角色**
| 优先级 | 位置 | 有球角色 | 无球角色 | 信心 | 原因 |
| --- | --- | --- | --- | --- | --- |

**战术建议**
<适合的阵型/节奏/压迫高度/搭档类型，以及不适合的用法>

**个人训练**
<IP/OOP 角色关注 + 额外关注 + 可考虑/避免的习惯>

**管理建议**
<首发/轮换/出租/观察/买入价位逻辑/出售逻辑>
```

Shorten the template when the user asks for a quick take.
