Companion: 11 · Give AI the context your team already has
Purpose: Bring the problem, people, evidence, constraints and success conditions into a linked brief.

# Give AI the context your team already has

## Run this resource on its own

1. Open an assistant approved by your organization for this material, such as an approved Cursor chat, Claude, or ChatGPT workspace. Use a read-only or drafting mode. No integration, installed command, or background automation is required or assumed.
2. Attach this complete Markdown file, or paste its entire text into the conversation. Then use the short invocation below. Alternatively, copy a complete prompt block from this file with your inputs; required templates are included in the relevant prompt.
3. Supply an exact issue ID or pasted issue text, or a clearly bounded topic; approved brief, research excerpts, prototype/flow, decisions and constraints; any known owner and outcome. Attach approved files or paste labeled excerpts with source names, dates and locations. A link is usable only if the assistant can actually read it. Redact personal or restricted details under your organization's rules; never include credentials.
4. Ask it to list what it could inspect before drawing conclusions. If essential inputs are missing, keep the output provisional and ask for the smallest useful evidence or access request. Missing evidence is not a finding.
5. Expect a source index and five-field context brief: problem, user/situation, evidence, constraints, success, plus conflicts and the next question. Check important claims against their sources and confirm decisions with the relevant people before using the draft.

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


LWT Field Kit · Yvonne Doll · Draft for review · Updated October 3, 2026

**Slides:** 11, “Give AI the context your team already has,” and 16, “My working system for design”  
**Format:** Linked brief and reusable prompt  
**Monday move:** Ask AI what it is missing before asking it for a solution.

## Use this as an index into the evidence

Open the current issue, brief, or rough prototype. Add links or approved excerpts from research, requirements, decisions, and relevant constraints. This brief points to the knowledge your team has; it does not replace the full record.

A rough idea or code experiment can come first. Before treating it as a product direction, have a person confirm the purpose and assumptions AI extracts from it.

Start with an exact Linear issue ID or URL when you have one. If you remember only the topic, first check that the assistant has an available, authorized issue connector. Search the relevant accessible project and return a short numbered shortlist with each issue's ID, title, and verified link. Let the person select the issue before assembling its context. A search match is not a confirmed target; read the selected issue and relevant linked sources.

If the connector or source access is unavailable, use pasted issue text, approved exports, and supplied excerpts. Say what is missing rather than implying an integration exists. Code can show implemented behavior; it does not establish the purpose, user need, or approval behind that behavior.

## Five fields

### Problem
What is happening that needs to change? Describe the difficulty without embedding your preferred solution. Who says this is a problem? What decision does the team need to make?

### User and situation
Who encounters it, while trying to do what? Include relevant roles, permissions, frequency, environment, or competing needs. Avoid invented personas.

### Evidence
What did we actually observe? Link the original source, date, scope, and limitation. Separate direct observation from an interpretation or repeated claim. Use [resource 01's claim-audit entrypoint](Slide_12_Audit_Claims_Carry_Evidence_and_Build_a_Decision_Brief.md#2-audit-consequential-claims) when a claim has lost its source.

### Constraints
What is fixed, negotiable, or unconfirmed? Include only relevant technical, accessibility, privacy, operational, commercial, and time constraints. Name who can confirm a constraint. “Someone said engineering can't do it” needs a source and an owner.

### Success
What should change for people and the business in this iteration? What signal can we actually inspect, when, and for which population? What decision will the result inform? A board demo may have a demonstration goal, but that does not establish a customer outcome.

## Copyable prompt

> Build a short context brief for this project from the material I explicitly provide or authorize. First list accessible sources and missing access. Use information already available in the current workspace; do not ask me to re-enter known context.
>
> If I give an exact issue ID or URL, resolve and read that issue. If I give only a topic, verify that an authorized issue connector is available, search only the relevant accessible project, and show a numbered shortlist with IDs, titles, and verified links. Ask me to choose before building the brief. If no connector is available, work from pasted text or approved exports and label missing access. Do not assume an integration or silently choose a similar issue.
>
> Fill Problem, User and situation, Evidence, Constraints, and Success. Attach a source and date to each material factual claim. Label unsupported interpretations as hypotheses and missing information as unknown. Preserve disagreements between sources. Do not turn the most recent or most polished document into the truth automatically.
>
> If a prototype came first, summarize what it appears to do and ask a person to confirm why it should exist. Do not infer approved purpose from implemented behavior.
>
> Ask the single missing question most likely to change the next decision. After my answer, update the brief and ask the next necessary question. Avoid a long intake form. Return a source index, the five fields, unresolved conflicts, and the human owner needed for each important gap. Stop before proposing or building a solution unless I ask.

## Output record

- Project / issue / artifact version:
- Brief owner and last checked date:
- Problem:
- User and situation:
- Evidence, with source IDs:
- Constraints, with confirming owners:
- Success for this iteration:
- Most consequential unknown:
- Conflicting information:
- Next question and person who can answer:

For each source, retain title/link or supplied excerpt ID, date, original author/owner if known, coverage, and any access limitation. Do not expose restricted material to reviewers who cannot access it.

## Fictional example

**Problem:** Administrators hesitate before activating an agent.  
**Evidence:** Two supplied interview excerpts describe uncertainty about its permissions. They do not establish how common the problem is.  
**Constraint:** The security review requires a permission check, confirmed in a dated decision record.  
**Unknown:** Is hesitation mainly about permissions, expected behavior, or something else?  
**Next question:** Which part of activation do people need to understand or verify before proceeding?

A button redesign is one possible intervention. The brief keeps the team from quietly assuming it is the answer.
