Companion: 16 · My working system · optional
Purpose: Clarify what this iteration is for and what readiness means.

# Start a project by asking done for what

## Run this resource on its own

1. Open an assistant approved by your organization for this material, such as an approved Cursor chat, Claude, or ChatGPT workspace. Use a read-only or drafting mode. No integration, installed command, or background automation is required or assumed.
2. Attach this complete Markdown file, or paste its entire text into the conversation. Then use the short invocation below. Alternatively, copy a complete prompt block from this file with your inputs; required templates are included in the relevant prompt.
3. Supply project description; new idea/prototype/existing-feature status; next intended use; artifact/version; approved evidence and constraints; known owner and deadline, or unknown. Attach approved files or paste labeled excerpts with source names, dates and locations. A link is usable only if the assistant can actually read it. Redact personal or restricted details under your organization's rules; never include credentials.
4. Ask it to list what it could inspect before drawing conclusions. If essential inputs are missing, keep the output provisional and ask for the smallest useful evidence or access request. Missing evidence is not a finding.
5. Expect a draft iteration agreement with purpose, real/simulated behavior, readiness and learning conditions, open decisions and the next action. Check important claims against their sources and confirm decisions with the relevant people before using the draft.

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


LWT Field Kit · Yvonne Doll · The New Design Surface  
Draft for review · Updated October 3, 2026  
Optional framing aid in slide 16, “My working system for design.” The iteration-purpose example in slide 14 is a narrower use; this file does not cover the full AI-behavior topic

## Purpose

Agree on what the next iteration needs to achieve before its polish starts making promises for you. A board demonstration, a learning experiment, a client review, and a production release need different things to be real.

Use this resource to turn an idea, an existing feature, or a rough prototype into a small, useful agreement: what we are trying to learn or accomplish, what is simulated, what must work, and who makes the next decision.

You can start with a prototype. A sketch or rough working example can make the question easier to see. The brief can follow it. What matters is that people confirm the purpose and assumptions before the prototype is treated as a commitment.

**This Markdown file is a worksheet and reusable prompt.** It does not create a project, connect to your tools, run tests, send messages, or install an automation.

## When to use it

- You are starting something new and have more ideas than shared context
- Someone says “it is almost done,” but the team means different things by “done”
- An existing feature needs a change and you do not yet know which behavior must stay intact
- A polished prototype is being mistaken for release-ready software
- The purpose changes, such as a demo becoming a customer pilot

Keep the first pass short. Answer the few questions that change the next step. Leave a question explicitly open when answering it would require research you have not done.

## How to use it

1. Name the next use of the work. Choose a concrete situation, such as “a five-minute board demonstration of one workflow” or “a moderated test of whether first-time admins understand activation.”
2. Bring what exists: a sketch, prototype, issue, brief, research excerpt, or a description from the person who started the work. Do not delay a useful conversation to complete a template.
3. Use the prompt below. Give the assistant only material your organization permits that assistant to access. A link alone does not guarantee it can read the source.
4. Confirm the resulting purpose and readiness conditions with the people whose expertise could change them. Name a decision owner.
5. Keep the agreement beside the prototype. Update it when the purpose, evidence, constraints, or risks change.

## The first questions

Ask these progressively rather than turning kickoff into an intake exam.

### Start with the next iteration

- What will someone do with this iteration, and when?
- What decision, learning, or customer capability should it enable?
- Who is the human owner of that decision?
- What would make this iteration misleading or unsafe for that use?

### If the feature is new

- Who encounters the problem, in what situation, and what are they doing today?
- What evidence suggests this is worth pursuing? Which parts are assumptions?
- What is the smallest scenario that could change our mind?
- What constraints are already real: data, permissions, platforms, cost, policy, or existing commitments?

### If the feature already exists

- What currently happens, for whom, and where does it fail?
- What must keep working for current users?
- Which previous decision or constraint might explain the behavior?
- What could this change affect elsewhere, including saved data, access, integrations, and support?
- What baseline or existing evidence will help us judge the change?

### Then make the agreement concrete

- Which data, actions, responses, and integrations are simulated?
- Which end-to-end paths must work for this use?
- Which failure and recovery paths matter now?
- What evidence will show that we built what we intended?
- What separate evidence will show whether it helped?

Do not make every question a prerequisite for a rough sketch. Elevate questions as consequences increase.

## Match readiness to the actual purpose

| Intended use | A useful readiness agreement | A limit to make visible |
| --- | --- | --- |
| Board demonstration | One named story runs reliably; the presenter can explain what is real; screenshots or a reset path are available if the demo fails | A successful demonstration does not establish customer value, scalability, or release readiness |
| Learning experiment | The critical interaction is credible enough to test the assumption; participants and conditions are appropriate; the team knows what result could change its plan | Only the tested question is supported; simulated behavior may limit what can be learned |
| Client preview or review | The audience, feedback question, approved material, and simulated parts are explicit; nobody could reasonably mistake a preview for a contractual promise | Showing an experience can create expectations even when the code is temporary |
| Production release, including a client-specific release | Relevant behavior, access, error handling, data handling, accessibility, operational ownership, and release controls are checked by the responsible people | A checked implementation still needs post-release evidence of usefulness and business effect |

These are starting points. Your team must set readiness conditions for the actual risk and context. A limited rollout may still handle real data or produce real consequences.

## Paste ready prompt

Copy the prompt and replace the bracketed fields. You can answer “unknown” without inventing detail.

```text
Help us define the next iteration of this project. Begin by asking “Done for what?” Keep the work open to product, design, and engineering input.

Project or feature: [name and short description]
Starting point: [new idea / rough prototype / existing feature / other]
Next intended use: [board demonstration / learning experiment / client preview / production release / unknown]
Current artifact: [attach it, paste a description, or provide an accessible link]
Available context and sources: [brief, issue, evidence excerpts, decisions, constraints]
Known owner and people involved: [names or roles; unknown is acceptable]
Time or scope constraint: [constraint or unknown]

Work this way:
1. Use relevant context already available in the current permitted workspace rather than asking the author to repeat it or identify a repository you can already see. First list what you can actually inspect. Separate inspected material, my description, and unavailable sources. Never imply that you read a link, repository, research file, or analytics source you cannot access.
2. Ask at most three high-value questions at a time. First establish the intended use, the decision or learning it should enable, and a human decision owner. If the purpose is unclear, help distinguish the plausible choices rather than assuming production readiness.
3. Adapt the next questions. For something new, ask about the person, problem, current workaround, evidence, and smallest useful experiment. For an existing feature, also ask about current behavior, regression risks, prior decisions, constraints, baseline evidence, and affected neighboring workflows.
4. A rough prototype may come before the brief. Inspect what exists and draft a tentative explanation of its purpose, assumptions, and behavior. Label this as your interpretation until a person confirms it. Do not reverse-engineer polished screens into settled requirements.
5. Draft a compact iteration agreement using the included output template. Separate observed facts, interpretations, assumptions, and open questions. Keep a source and date attached to consequential claims when available. Flag contradictions rather than silently choosing a source.
6. Make the real-versus-simulated boundary explicit for data, actions, integrations, permissions, and failure handling. Identify anything that the audience could reasonably misunderstand as working.
7. Propose observable readiness conditions for the intended use. Distinguish conformance checks from evidence that the experience helps people. Say what will remain untested. Treat readiness and risk levels as proposals for the responsible people to confirm.
8. End with the smallest useful next action, its proposed owner, and the question it resolves. Ask for confirmation before treating the iteration agreement as approved.

Stay within this drafting task. Do not edit a shared issue, publish the artifact, contact reviewers, activate a feature, create reminders, or change production systems. If additional access or an action is needed, describe it and ask the owner.

Output: an iteration agreement, no longer than necessary to guide the next decision, followed by the few unresolved questions that could change it.

OUTPUT TEMPLATE
# Iteration agreement

Project: [name]
Version and date: [version, date]
Human decision owner: [name; confirmation status]
Contributors needed now: [people or roles and why]

## Done for what
Next intended use: [specific audience and situation]
Decision or learning enabled: [the question this iteration should answer]
User outcome sought: [what should become easier, possible, or safer]
Business reason: [why the change matters; mark hypotheses]

## Context we are using
- [Claim; observed, inferred, or assumed; source and date; limitation]
- Unavailable or missing context: [what is missing and why it matters]
- Contradictions to resolve: [conflicting claims or none found in inspected material]

## This iteration
Included scenarios: [specific paths]
Outside this iteration: [explicit exclusions]
Existing behavior to preserve: [behavior or not applicable]
Real behavior: [what actually works]
Simulated behavior: [what is staged and how it will be disclosed]

## Readiness conditions
- [Observable condition; check method; responsible person; current status]
- [Observable condition; check method; responsible person; current status]
Untested or deferred: [limits and consequence]

## Learning conditions
Evidence we will collect: [observation or measure; source; timing]
Result that could change our plan: [decision rule or interpretation question]
What the evidence cannot establish: [limits]

## Open decisions and next action
- [Decision; human owner; evidence needed; due date or next decision point]
Next action: [small action; owner; completion signal]
Approval status: [draft / confirmed for this purpose by name and date]
Revisit when: [purpose, evidence, scope, or risk change that requires a new check]
```

## Output template

```markdown
# Iteration agreement

Project: [name]
Version and date: [version, date]
Human decision owner: [name; confirmation status]
Contributors needed now: [people or roles and why]

## Done for what
Next intended use: [specific audience and situation]
Decision or learning enabled: [the question this iteration should answer]
User outcome sought: [what should become easier, possible, or safer]
Business reason: [why the change matters; mark hypotheses]

## Context we are using
- [Claim; observed, inferred, or assumed; source and date; limitation]
- Unavailable or missing context: [what is missing and why it matters]
- Contradictions to resolve: [conflicting claims or none found in inspected material]

## This iteration
Included scenarios: [specific paths]
Outside this iteration: [explicit exclusions]
Existing behavior to preserve: [behavior or not applicable]
Real behavior: [what actually works]
Simulated behavior: [what is staged and how it will be disclosed]

## Readiness conditions
- [Observable condition; check method; responsible person; current status]
- [Observable condition; check method; responsible person; current status]
Untested or deferred: [limits and consequence]

## Learning conditions
Evidence we will collect: [observation or measure; source; timing]
Result that could change our plan: [decision rule or interpretation question]
What the evidence cannot establish: [limits]

## Open decisions and next action
- [Decision; human owner; evidence needed; due date or next decision point]
Next action: [small action; owner; completion signal]
Approval status: [draft / confirmed for this purpose by name and date]
Revisit when: [purpose, evidence, scope, or risk change that requires a new check]
```

## Worked fictional example

**Project:** Relay, a fictional tool that helps support administrators configure an AI assistant. All people, observations, and records below are invented for illustration.

**Starting point:** A designer built a rough prototype over a weekend. It offers a prominent “Publish” button. A short product note says an administrator must test the assistant before activation. Nobody has agreed on the meaning of “Publish.”

### The first exchange

Assistant: “Who will use this iteration, what decision should it help you make, and who owns that decision?”

Author: “We want to show it to four support administrators in moderated sessions next week. We need to learn whether they understand the difference between testing and activation. Mira, our PM, owns the next scope decision.”

Assistant: “Does this prototype contact customers or change live settings? What is simulated? Can I inspect the product note as well as the prototype?”

Author: “It uses fictional tickets and fixed responses. No customer contact or live settings. Here is the note.”

### The resulting agreement

- **Done for:** A learning experiment about the activation model, with four exploratory sessions. This small sample will help identify problems and questions; it will not estimate how common they are across all administrators
- **Evidence:** The supplied product note requires a test before activation. The prototype has a direct Publish action. This is an observed contradiction between two artifacts, not proof that either approach is right
- **Owner:** Mira confirms the experiment's purpose. Jules, the designer, owns the session scenario. An engineering representative checks the representation of testing and activation before the sessions
- **Included:** Configure an assistant, run a sample test, inspect its result, correct the configuration, and explain what would happen on activation
- **Real:** Navigation, editable sample instructions, and clear state changes within the local prototype
- **Simulated:** Ticket data, assistant responses, saving, permissions, and activation. The introduction identifies it as a prototype with fictional data; the activation screen says it will not go live
- **Readiness:** Every participant can enter the same starting state; the test result can be reset; the Publish contradiction is resolved for the scenario; no action can reach a real customer; the researcher can distinguish participant understanding from coaching
- **Conformance check:** The scripted test-before-activation path works, including returning to edit after an unsatisfactory result
- **Learning check:** Ask participants to explain the difference between a test and activation and show what they would do after a failed test. Record misunderstandings and the point where they occur
- **Decision:** If people still confuse a test with going live, revise the activation model before expanding the prototype. Mira interprets the observations with design and engineering; the assistant does not issue a pass or fail verdict
- **Untested:** Actual model performance, production permissions, infrastructure, reliability, and customer outcomes
- **Next action:** Jules changes the direct Publish action into the agreed test scenario and brings the revised path back to Mira and engineering before recruitment begins

The team can now improve the prototype without pretending the whole product has been specified.

## Limitations and permissions

- An assistant can help expose gaps. It cannot establish a user's need, a system's safety, or release readiness from a convincing screen
- Use only permitted sources and tools. Redact customer information or use synthetic examples when broader access is unnecessary
- This prompt authorizes a draft, not publication, external sharing, live testing, or production changes
- If the intended use changes, reassess readiness. A learning prototype does not inherit permission to become a live pilot
- Keep a human owner for commitments, severity judgments, and the decision to proceed

## Monday move

Choose one current prototype. Ask “What must this iteration achieve?” Write one sentence for its purpose, one sentence naming what is simulated, and three observable readiness conditions. Get the decision owner to confirm those before adding more polish.
