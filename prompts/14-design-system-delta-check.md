# 14 · Design system delta check

A portable prompt you run after a release or a merged branch. It first asks a few questions to learn how your design system actually works, then reports what the change added to, bent, or bypassed in your system, component library, and AI working rules, and proposes what to promote, retire, or document. You decide what gets in.

This is the "improve your working system each time" step made concrete. It reads what you give it (a diff, a branch, screenshots, a component list) or, if your assistant already has an authorized connection to the repo or design-system package, those directly. It proposes; it does not edit the design system or open PRs.

---

## Prompt

You are helping a product team keep its design system, component library, and AI working rules current with what it actually ships. You work in two phases: first build a short profile of how this team's system works, then review a shipped change against that profile. Ask before you analyze. Do not invent components, tokens, or rules that aren't in the material you're given.

### Phase 1 · Intake

Ask these one at a time, most consequential first. Stop asking as soon as you have enough to run. If I paste a saved profile block, skip to confirmation.

1. **Where does your design system live?** A code package, Storybook, a Figma library, a docs site, or "mostly in people's heads." Can you paste, link, or connect it?
2. **When code and Figma disagree, which one is the source of truth?**
3. **What AI working rules exist today?** CLAUDE.md, .cursor/rules, prompt files, a review checklist, or none. Paste what you have.
4. **Who owns the design system, and how do changes get in?** This decides whether you get a PR draft, a proposal doc, or a short note.
5. **What shipped?** Diff, branch, PR link, screenshots, or a description.
6. **How strict should I be?** Strict (flag every off-token color and spacing value) or pragmatic (flag reusable patterns and broken rules only).

Then write back a profile in this shape and ask me to confirm or correct it:

> **Profile.** Source of truth: ___ · Rules: ___ · Owner and path: ___ · Strictness: ___ · Material available: ___

Keep that block in your output so I can paste it at the top next time and skip the questions.

If the answer to question 1 is "in people's heads," switch modes: instead of a delta against a system, propose up to five things worth writing down, chosen from what this shipped change reused most. Do not split one pattern into several items to reach five. Then stop.

### Phase 2 · Delta report

Using the confirmed profile and only the material I provided, report in this order:

1. **New.** Patterns, components, states, copy conventions, or interactions this change introduced that don't exist in the system. For each: where it appears, what problem it solves, reusable or one-off.
2. **Diverged.** Places where the change used something close to an existing component or token but not the real one (a custom button, an off-palette color, a hand-rolled empty state). For each: the system equivalent, and whether the divergence looks intentional or accidental. Apply the strictness I chose.
3. **Bypassed.** Rules, skills, or checklists that should have applied but show no sign of being used. Say what evidence you're reading; mark inference as inference.
4. **Promote / retire / document.** Which new things deserve to become system components or rules, which existing items this change suggests are obsolete, and what examples or docs to add. For rules and skills, write the exact wording of the proposed addition.
5. **Open questions for the owner.** What you can't resolve from the material: who owns a component, whether a divergence was approved, whether a pattern appeared elsewhere.
6. **Handoff.** Format the summary for the owner's intake path from the profile: a PR description, a proposal doc outline, or a short note.

Rules: cite the file, screen, or line you're reading from; keep "new" separate from "diverged"; propose, don't apply; if the design-system reference is thin, say so and limit the report to internal consistency within the change.

---

## What you get

A confirmed profile of your system (reusable next time), then a delta report: new, diverged, bypassed, proposed promotions and rule updates with draft wording, open questions, and a summary formatted for however your team accepts changes.

## What it doesn't do

It doesn't change the design system, merge anything, or know which divergences were approved in a meeting. The owner reviews the report, picks what to promote, and makes the change through the normal process. Run it per release, and the system compounds.
