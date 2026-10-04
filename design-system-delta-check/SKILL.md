---
name: design-system-delta-check
description: After a release or merged branch, build a short profile of the team's design system and AI rules, then report what the change added, diverged from, or bypassed, and propose what to promote, retire, or document. Use when the user asks to check a shipped change against the design system, find new or off-system components, or update rules and skills after a project.
---

# Design system delta check

Work in two phases. Ask before you analyze. Never edit the design system, open PRs, or invent components, tokens, or rules that aren't in the material you're given.

## Phase 1 · Intake

Ask these one at a time, most consequential first. Stop as soon as you have enough to run. If the user pastes a saved profile block, skip straight to confirmation.

1. Where does your design system live? (code package, Storybook, Figma library, docs site, or "mostly in people's heads") Can you paste, link, or connect it?
2. When code and Figma disagree, which is the source of truth?
3. What AI working rules exist today? (CLAUDE.md, .cursor/rules, prompt files, review checklist, none) Paste what you have.
4. Who owns the design system, and how do changes get in? (decides output format: PR draft, proposal doc, or short note)
5. What shipped? (diff, branch, PR link, screenshots, or description)
6. How strict should I be? Strict (every off-token value) or pragmatic (reusable patterns and broken rules only).

Write back a profile and ask the user to confirm or correct it:

> **Profile.** Source of truth: ___ · Rules: ___ · Owner and path: ___ · Strictness: ___ · Material available: ___

Keep that block in the output so the user can paste it next time.

If the answer to question 1 is "in people's heads," switch modes: propose up to five things worth writing down, chosen from what the shipped change reused most. Do not split one pattern into several items to reach five. Then stop.

## Phase 2 · Delta report

Using only the confirmed profile and the provided material, report in this order:

1. **New.** Patterns, components, states, copy conventions, or interactions the change introduced that don't exist in the system. Where it appears, what problem it solves, reusable or one-off.
2. **Diverged.** Near-misses of existing components or tokens (custom button, off-palette color, hand-rolled empty state). The system equivalent, and whether the divergence looks intentional or accidental. Apply the chosen strictness.
3. **Bypassed.** Rules, skills, or checklists that should have applied but show no sign of use. State the evidence; mark inference as inference.
4. **Promote / retire / document.** What should become a system component or rule, what looks obsolete, what examples or docs to add. For rules and skills, write the exact proposed wording.
5. **Open questions for the owner.** Ownership, whether a divergence was approved, whether a pattern appears elsewhere.
6. **Handoff.** Format the summary for the owner's intake path from the profile.

## Rules

- Cite the file, screen, or line you're reading from.
- Keep "new" separate from "diverged."
- Propose; don't apply.
- If the design-system reference is thin, say so and limit the report to internal consistency within the change.
- If the assistant has an authorized connection to the repo or design-system package, read it within the scope the user confirms; otherwise work from pastes and exports. Do not claim access you don't have.
