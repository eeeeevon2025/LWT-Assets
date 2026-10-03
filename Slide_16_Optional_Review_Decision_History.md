Companion: 16 · My working system · optional
Purpose: Review prior decisions, their evidence and what has changed.

# Trace a workflow decision before redesigning it

## Run this resource on its own

1. Open an assistant approved by your organization for this material, such as an approved Cursor chat, Claude, or ChatGPT workspace. Use a read-only or drafting mode. No integration, installed command, or background automation is required or assumed.
2. Attach this complete Markdown file, or paste its entire text into the conversation. Then use the short invocation below. Alternatively, copy a complete prompt block from this file with your inputs; required templates are included in the relevant prompt.
3. Supply the workflow and decision to revisit; approved current/earlier artifacts with dates and release status; decision records, research and support evidence; search boundary and known owners. Attach approved files or paste labeled excerpts with source names, dates and locations. A link is usable only if the assistant can actually read it. Redact personal or restricted details under your organization's rules; never include credentials.
4. Ask it to list what it could inspect before drawing conclusions. If essential inputs are missing, keep the output provisional and ask for the smallest useful evidence or access request. Missing evidence is not a finding.
5. Expect a sourced decision timeline, recorded versus inferred reasons, what changed, what still holds, and a neutral question for the biggest gap. Check important claims against their sources and confirm decisions with the relevant people before using the draft.

**Copy this invocation after attaching or pasting this file:**

```text
Use the attached/pasted resource instructions for this bounded task.
My project, decision, or question: [fill in]
My chosen route, if this resource offers more than one: [fill in]
Approved inputs and their source names/dates: [attach or paste here]
Permitted source/access boundary: [fill in; supplied material only is fine]
Known constraints and human owner: [fill in or unknown]
Return the output specified in this resource. First say which inputs you can
actually read. Preserve source references, contradictions and uncertainty.
If evidence is missing, draft the next question or evidence request instead
of inventing results. Treat examples as fictional demonstrations, not evidence
about my project. Draft only; do not send, install, execute, change access,
change tracking, or modify project/production records.
```


Yvonne Doll · The New Design Surface · LWT Field Kit

Draft for review · Updated October 3, 2026

**Format:** Reusable prompt and worksheet; skill-body draft where a host supports it

## Optional context for the lifecycle example

**Optional during Understand on slide 16, “My working system for design”; there is no dedicated slide.** When you are assigned to improve an existing workflow, reconstruct what was tried, why it changed, and what evidence would make a different choice reasonable now. The result should help you design the next iteration without treating the current experience as an accident or a past attempt as a permanent veto.

**What you make:** A source-backed decision timeline and a short “what is different now” brief. Start with one consequential decision, not the entire product history. Allow 30–45 minutes for the first pass; missing records may require an owner's input.

## Gather these inputs

- The assigned workflow, people affected, current problem, and decision you need to make
- Current and earlier designs or prototypes, with dates and version labels if available
- Relevant issues, release notes, decision records, research findings, support themes, and measurement summaries
- Known decision owners or participants who can resolve gaps
- A clear time and product boundary for the search

Use authorized sources in an approved AI environment. Old research may include personal data; use approved excerpts or aggregate findings where possible. A file name or screenshot alone may not establish what shipped.

## How to use it

1. **Name the decision.** For example: “Can identity verification move later in onboarding?” This focuses the search more effectively than “Why is onboarding bad?”
2. **Collect the visible versions.** Distinguish proposed, tested, approved, released, rolled back, and superseded. Do not turn every design exploration into a production event.
3. **Run the prompt.** Ask AI to assemble a timeline and label every reason as recorded, inferred, or unknown.
4. **Verify the pivotal transition.** Open the source for the change most relevant to your current proposal. Check chronology, user group, release status, and the evidence available at that time.
5. **Resolve one important gap.** Ask an appropriate owner for the missing reason or constraint. Their current recollection is useful testimony; label it as retrospective and keep it distinct from a contemporary record.
6. **Write the present-day choice.** Identify what has changed, what still holds, and the next evidence needed. Use this to scope an experiment or proposal rather than declaring an earlier team wrong.

## Copyable AI prompt

```text
I am a designer assigned to improve an existing workflow. Help me understand
its decision history before proposing a redesign.

Workflow and affected people: [description]
Current user problem: [description and evidence]
Decision I need to make: [specific question]
Search scope and time period: [boundaries]
Permitted sources: [links, exports, or pasted material]
Known owners or participants: [names and roles, or unknown]

First state which sources you can actually read and what is missing. Analyze
only permitted material. Do not claim a complete history if coverage is partial.

Build a chronological account of relevant versions and transitions. For each:
- Version/date and whether it was proposed, tested, approved, released,
  rolled back, or superseded; mark ambiguous status as unknown
- What changed for which users
- The recorded decision and named owner, if documented
- The reason recorded at that time, with source and section
- Evidence available then, including its method, population, and limitations
- Observed result, if measured, with source and observation window
- Constraints, alternatives considered, and unresolved disagreement

Separate recorded reasons, your inferences, and unknowns. If sources conflict,
show the conflict; do not silently choose a convenient explanation. Do not
infer motive, blame, or causal impact from the sequence of events. Keep
retrospective recollections distinct from contemporary evidence.

Then compare the earlier situation with today: users, problem, policy,
technical capability, economics, market, and measurement. Mark each proposed
difference as verified, plausible but unverified, or unknown. State which
prior constraint still holds and what evidence would change our present choice.

Return the timeline, three most consequential gaps, and a brief using the
included output template. Draft a neutral owner question for the biggest gap.
Do not send messages or edit project records. Do not recommend a redesign
solely because a prior design looks dated or because one metric moved.

OUTPUT TEMPLATE
DECISION HISTORY BRIEF
Workflow / current problem / decision under consideration:
Researcher / review date / search boundary:
Sources checked / sources missing:

TIMELINE ENTRY
Version and date / status and evidence of status:
Affected people and experience:
Decision / documented owner:
Recorded reason / source and section:
Evidence available then / limitations:
Observed result / population and window / source:
Inference, clearly labeled:
Unknown or conflicting record:

WHAT IS DIFFERENT NOW
Earlier condition:
Present condition / supporting source:
Status: verified, plausible but unverified, or unknown
Implication for this decision:

WHAT STILL HOLDS
Constraint or useful lesson / source / owner to confirm:

NEXT DECISION
Option worth evaluating:
Evidence that would support or rule it out:
Most important gap / question / person to ask:
Decision owner / next step / review date:
```

## Output template

```text
DECISION HISTORY BRIEF
Workflow / current problem / decision under consideration:
Researcher / review date / search boundary:
Sources checked / sources missing:

TIMELINE ENTRY
Version and date / status and evidence of status:
Affected people and experience:
Decision / documented owner:
Recorded reason / source and section:
Evidence available then / limitations:
Observed result / population and window / source:
Inference, clearly labeled:
Unknown or conflicting record:

WHAT IS DIFFERENT NOW
Earlier condition:
Present condition / supporting source:
Status: verified, plausible but unverified, or unknown
Implication for this decision:

WHAT STILL HOLDS
Constraint or useful lesson / source / owner to confirm:

NEXT DECISION
Option worth evaluating:
Evidence that would support or rule it out:
Most important gap / question / person to ask:
Decision owner / next step / review date:
```

Repeat the timeline entry for each consequential transition. If a reason cannot be found, write “not documented in the sources checked.” That is more useful than a polished invented explanation.

## Worked fictional example

All names, records, dates, and findings in this example are invented.

**Assignment:** Improve onboarding for business account administrators at Cedar. The designer is considering moving identity verification until after workspace setup.

**Version 1, January:** Verification precedes workspace setup. A January decision record says access to customer records requires verified identity. The document names Arun as the decision owner. This is a recorded access-control requirement, not evidence that early verification is the best user experience.

**Version 2, March:** A prototype moves verification later. Five usability sessions suggest participants understand the first setup task more easily. The prototype was tested, but no release record was found. The sample and test setting cannot establish a change in real-world activation.

**Version 3, April:** The released flow retains early verification. An April issue records a technical limitation: an unverified administrator could enter a workspace containing customer data. There is no documented production rollout or rollback of Version 2. Calling this “we removed verification and had to restore it because users failed” would invent both events and a cause.

**Current state, September:** Engineering documentation describes a sandbox workspace that cannot access customer records before verification. The designer has not yet confirmed that the sandbox is available to this onboarding flow. Its relevance is plausible but unverified.

**What is different now:** A new technical capability may allow useful setup before verification. The requirement to verify identity before customer-data access still holds. The March research provides a hypothesis about comprehension, not proof of a production benefit.

**Owner question:** “Arun, the April issue says verification stayed early because unverified administrators could reach customer data. Does that constraint still apply to the new sandbox, and who can confirm its access boundaries?”

**Next step:** Ask engineering to validate sandbox behavior and the appropriate policy owner to confirm the access requirement. If both support the idea, test a sandbox-first journey with representative administrators, including people who cannot complete verification. Preserve a clear path back to incomplete verification. The decision remains open until those checks are complete.

## Optional separate leadership rework audit

This is a different question from a designer's workflow investigation. Use it only when a leader wants to understand repeated work over a defined six-month period. It must not become an individual performance score or a tally of “bad decisions.”

**Scope the review:** Name the product area, exact six-month dates, records available, and the definition of rework. A useful working definition is a material revision to work previously approved or released. Include the number of projects reviewed so the reader can judge coverage. Do not extrapolate from a handful of memorable reversals to the whole organization.

**Classify each episode using evidence:**

- **Potentially preventable coordination failure:** Relevant evidence or a constraint existed and could reasonably have reached the decision before commitment, but the record suggests it did not. Confirm with involved owners before calling it preventable.
- **Rational learning:** The team changed direction because useful evidence emerged from a test, release, or research that was not reasonably available earlier.
- **Changed conditions:** A policy, market, customer, business, or technical condition changed after the earlier decision.
- **Mixed or unresolved:** More than one explanation applies, or records cannot establish the reason.

Record source, timing, owner validation, and confidence for every classification. Ask what information was reasonably knowable then; do not judge the earlier decision using only today's knowledge. Do not assign all development cost to rework or estimate “waste” from ticket counts. Include time or cost only if the responsible team validates the method and estimate.

### Optional leadership prompt

```text
Review material revisions in [product area] from [start date] to [end date],
an exact six-month period, using only [permitted sources]. Our definition of
rework is [definition]. List the projects included and missing coverage.

For each episode, reconstruct the original decision, information available
then, later trigger, and evidence for the revision. Classify provisionally as
potentially preventable coordination failure, rational learning, changed
conditions, or mixed/unresolved. Explain the evidence and what owner
confirmation is still needed. Never present inferred causes as facts.

Separate repeated coordination patterns from reasonable adaptation. Do not
rank people, infer motives, or invent time/cost savings. Produce a short
episode register plus one process change to test, with an owner, a way to
observe whether it helps, and a review date. Do not modify team records.
```

**Fictional leadership example:** A later security review uncovered a known access constraint that an earlier design review did not include. That is a candidate coordination problem; confirm whether the constraint was documented and accessible before commitment. A second project changed after a new customer segment emerged. That may be reasonable adaptation. Counting both as “avoidable rework” would hide the very distinction the review is meant to reveal.

## Guardrails

- A design version is not evidence of a release.
- The order of events does not establish why a decision changed.
- A past failed attempt does not prove a current proposal will fail; ask which conditions differ.
- A past successful result does not guarantee the same result for different users or conditions.
- Missing documentation is a gap to investigate, not proof of poor judgment.
- Keep decisions and constraints visible without turning the history into a blame narrative.

## Monday move

Trace one past decision in your assigned workflow to its evidence. Ask the relevant owner whether the recorded reason still holds before redesigning around it.
