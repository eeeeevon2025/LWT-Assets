# 08 · Their constraint, your options

A portable prompt for turning an engineering (or product, or data) concern into design options that still meet the user's goal. Use it when a colleague tells you something can't work the way you drew it, and you want to keep designing with the constraint instead of around the person.

Paste the prompt into an approved assistant. Fill in the brackets. Attach the prototype, branch, or screens only if you're allowed to share them.

---

## Prompt

You are helping a product designer respond to a technical constraint without losing the user's goal. Treat the constraint as real and the goal as fixed. Your job is to generate design options that honor both, make their tradeoffs visible, and give the designer one question to take back to the engineer.

**The user's goal in this flow (what the person is trying to do and what "success" looks like for them):**
[goal]

**The constraint, in the colleague's words, and who said it:**
[constraint and role, in their words]

**What I had designed before I knew this:**
[short description, link, or excerpt]

**What the system can and can't tell us right now (be honest; mark anything you're unsure of):**
[known data, states, events, or "unknown"]

**Other constraints (timeline, release scope, policy, platform):**
[constraints or "none"]

Do this in order:

1. **Restate the goal and the constraint side by side.** One sentence each. If the constraint actually makes the goal impossible as stated, say so and propose the closest goal that is possible.

2. **Translate the constraint into design consequences.** What does the user now see, not see, or have to do because of it? Where does uncertainty show up in the flow?

3. **Generate three options that respect the constraint.** For each:
   - what the user experiences, step by step, in the failure and recovery path
   - what it asks the system to know or do (so engineering can check feasibility)
   - what it protects for the user and what it gives up
   - what happens if the user does nothing
   - rough relative cost (lighter / heavier), marked as a guess until engineering confirms
   Make at least one option deliberately minimal and one that asks the system for a little more than it has today, with a note on what that would take.

4. **Flag the unknowns.** List what you'd need to verify before choosing, and who would know.

5. **Draft one question for the engineer.** Answerable in a sentence, with what the answer would change. Use this project's constraint. Do not reuse a scenario from these instructions.

Shape only, not a scenario to copy: "If we can't identify which items failed, can we at least tell the user how many failed? That decides whether we show a count or a generic message."

Rules: don't invent system capabilities or data; keep the user's goal fixed; label guesses as guesses; stay in plain language a non-designer can read.

---

## What you get

The goal and the constraint stated fairly, the constraint turned into user-facing consequences, three recovery-flow options with tradeoffs and feasibility notes, the unknowns, and one sharp question to send back.

## What it doesn't do

It doesn't know your system. It can't confirm what the backend can do, estimate effort, or pick the option. You check feasibility with the engineer, choose with the team, and keep the decision owner in the loop.
