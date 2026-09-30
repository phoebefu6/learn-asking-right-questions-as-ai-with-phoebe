# learn-asking-right-questions-as-ai-with-phoebe - source map

Internal build document. Not linked from any audience-facing page.

Bucket `ai`, difficulty 2, audience both, 6 sessions, single track, no code. One of four
sibling courses sharing one framework, one company and one simulator engine.

**The framework, the shared sources, their evidence tiers and the "never print" list live in ONE
place:** `learn-asking-right-questions-as-da-with-phoebe/materials/official-course-map.md`. Never
restate or fork them here. This file holds only what differs for the ai developer.

Built 2026-09-30.

---

## The role's request and widest door

Harbourline and Adeline Tan are the same constructed case as the DA course. Her request to the
ai developer: "Can AI answer the supplier WhatsApps? My three area managers spend half their day on them."

**Widest door: Current way.** An AI developer's output replaces or assists a human step. The facts that decide whether it is safe are the workflow as it happens today, which replies are lookups and which are decisions, how often the human catches an error, and who checks the output; they sit behind door 3.

Seams: `learn-ai-red-team` and `learn-ai-observability` own testing and watching a system that exists; `learn-ai-hr`, `learn-ai-office` and the aiap shelf own AI by function. This course owns the discovery meeting before anything is built. The honest nuance on the bench: for this bank the tuned order beats door order by only one point (55 vs 54), because the printed order already asks the lookups-versus-decisions question (a decision-door question that does the current-way work) by minute 12, and the one-in-twenty error rate arrives at minute 16. The page says so rather than inflating the gap. (Corrected 2026-09-30: an earlier brief said the printed order reaches the current-way door by minute 12; the bench transcript shows it does not.)

---

## The bench (`assets/asking-live.js`, byte-identical to the DA copy, + `assets/asking-bank-ai.js`)

Verified headlessly in node on 2026-09-30. 24 facts worth 69 points, 37 questions,
45-minute budget, cut at 20 minutes.

| Preset | Net value | After 20 min | Facts | Doors | False beliefs |
|---|---|---|---|---|---|
| ANTI: the efficient interview | 21 | -4 | 12 | 6 | 5 |
| The technical opener | 11 | 0 | 4 | 2 | 0 |
| Any order at all (mean of 200) | 30.1 | 14.3 | 12.8 | 5.4 | 2.5 |
| Six Doors, door by door | 54 | 22 | 18 | 6 | 0 |
| Six Doors, tuned for an AI developer (current way widest) | 55 | 23 | 18 | 6 | 0 |
| Ceiling (optimizer reads the sheet) | 63 | 32 | | | |

The ceiling order opens with the lookups-versus-decisions question, which a real interviewer could ask first; for this role the framework and the optimizer agree on the opener and differ on what follows.

Random: best 52, worst -1.

The five false beliefs a leading question records on this bank: "reply to suppliers automatically" (substitutions need a human by law), "orders are in English" (English, Malay and Chinese with nicknames), "there is an order table" (there is none), "mistakes are rare and cheap" (one in twenty, and a wrong drug is not cheap), "a new app" (they live in WhatsApp in a van).

**Findings claimed:** the ordering only (fast and jargon below random, random below the doors,
the role-tuned order at or above the printed order), and the mechanism (jargon costs minutes and
trust, leading questions record wrong beliefs, the most sensitive fact needs trust 3). Never the
numbers as facts about a real business.

---

## Sessions

Same arc as the DA course; session 1 of this course is a short role-framed page that links the
DA session 1 for the corridor and does not restate the six doors.

| # | Title | Role emphasis |
|---|---|---|
| 1 | The gap, from the AI developer's chair | the role's tune, the widest door, links the canonical Six Doors |
| 2 | The thread end to end, and its data | the same five-rung ladder, framed for what this role needs from it |
| 3 | The AI developer's questions, and the bench | this bank, this ladder |
| 4 | Teaching while you ask | the one concept per meeting for this role |
| 5 | Three projects, and the assistant that only drafts | three candidates fitted to this role's output |
| 6 | The mock meeting and the one-page brief | the brief with this role's block 4 |

---

## Design system

Palette: **emerald and plum.** Scaffolded from the DA course, every hex recomputed; 22 text-on-fill pairs
checked, 0 failures (lowest 4.5 after mid moved to #087A57).

| Token | Hex |
|---|---|
| deep | `#065F46` |
| primary | `#047857` |
| mid | `#087A57` |
| soft | `#A7F3D0` |
| tint | `#ECFDF5` |
| ink | `#0F231B` |
| muted | `#46605A` |
| faint / hairline | `#C3DDD3` / `#DAEBE4` |
| accent | `#8E2C6B` |
| accent-ink | `#6A1F50` |
| accent tint | `#FBE9F4` |
| paper | `#FBFEFC` |
| code-bg / code-ink | `#0F231B` / `#DAEBE4` |

Figure grammar: identical to the DA course's hand-drawn grammar with this palette substituted.
`PASSPORT_KEY` = `lwp-passport:asking-right-questions-as-ai`.
