Companion: 5 · There is no handoff
Purpose: Turn a rough concern into a focused question a colleague can answer.

# Prepare a useful review request

## Run this resource on its own

1. Open an assistant approved by your organization for this material, such as an approved Cursor chat, Claude, or ChatGPT workspace. Use a read-only or drafting mode. No integration, installed command, or background automation is required or assumed.
2. Attach this complete Markdown file, or paste its entire text into the conversation. Then use the short invocation below. Alternatively, copy a complete prompt block from this file with your inputs; required templates are included in the relevant prompt.
3. Supply the concern and decision; artifact/version and approved context; intended recipient/role, channel and relationship; a writing example if available; timing only if actually agreed. Attach approved files or paste labeled excerpts with source names, dates and locations. A link is usable only if the assistant can actually read it. Redact personal or restricted details under your organization's rules; never include credentials.
4. Ask it to list what it could inspect before drawing conclusions. If essential inputs are missing, keep the output provisional and ask for the smallest useful evidence or access request. Missing evidence is not a finding.
5. Expect one concise review-request draft, its focused question, context/link, and any missing confirmation; nothing is sent. Check important claims against their sources and confirm decisions with the relevant people before using the draft.

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

October 2, 2026 · Companion to slides 5 and 16: “There is no handoff” and “My working system for design”

**Who are you talking to, and who is this meant for?**

Start there. Then choose the channel and the one thing you need that person to help you resolve.

A designer brings the concern, the thinking, and the relevant context. AI can help formulate that into a clear, brief request: what I noticed, why I’m asking you, and what your answer would change. Choosing what to ask and presenting a point of view are part of design work. The wording should carry that thinking accurately.

Use this for an everyday Slack or Teams message to one colleague, or a short comment on the existing issue. A useful request can fit in a few sentences. You do not need a new meeting or a review from every discipline.

## Start with the person and the channel

- **Person:** Who can answer this question or make this decision? Use what you know about their responsibility and context. A title such as engineer, product manager, or C-level executive does not establish what they know, own, or need to hear
- **Channel:** Slack or Teams message, an existing Linear issue, or a question for a meeting already taking place. Use the place where this exchange belongs
- **Your thinking:** What did you notice? What concerns you? What are you leaning toward, and what is still uncertain?
- **Necessary context:** The exact artifact, version, state, or piece of evidence the person needs. Use a direct link when available; make sure the recipient can open it
- **Consequence:** What would their answer change about the design, scope, priority, or next check?

You may need an implementation constraint from an engineer, a priority decision from a product owner, or an investment decision from a leader. Ask that person about the actual decision they can help with. Do not translate every request into the same disciplinary checklist or assume an executive only wants a business metric.

## Copy paste prompt

Paste this into an approved assistant with your rough notes. Fill only the fields that matter; a few rough sentences may be enough. Reuse context already in the conversation instead of rewriting a brief.

```text
Help me prepare one useful review request. Use the rough notes and context
I have supplied; do not require every field below to be completed.

Start with: Who am I talking to, and who is this meant for?
If I have already supplied that context, use it rather than asking again.

PERSON AND CHANNEL
Recipient and relevant responsibility/context: [person; what they can help with]
Channel: [Slack, Teams, existing Linear issue, or an existing meeting]
Existing thread/issue, if relevant: [reference, or none]

MY THINKING
What I noticed and why it concerns me: [rough notes]
My current view or candidate change: [if I have one]
What I need this person to resolve: [question or uncertainty]
What their answer could change: [design, scope, priority, or next check]

NECESSARY CONTEXT
Artifact and version: [direct link/reference; relevant screen/state/step]
Evidence I have: [observation, reproduction, report, or supplied excerpt]
What I have not established: [unknowns or constraints]
Timing: [only a real agreed deadline or decision point, if one exists]

Draft the shortest request that retains the decision-relevant context.
For Slack/Teams, aim for a few sentences to this one person. For an issue
comment, keep the question beside the relevant artifact/version. For an
existing meeting, give me a short spoken setup and the same focused question.

- Use my supplied concern and point of view. Do not invent my reasoning,
  feelings, evidence, urgency, commitments, or the recipient’s preferences.
- If the recipient or essential purpose is missing, ask one focused question
  before drafting. If my notes already support a useful request, draft it.
- Preserve the necessary counts, state, and artifact version. Cite or link
  the smallest useful source. Do not pretend to inspect an inaccessible link.
- Distinguish what was observed from what might happen and what is unknown.
  If my claim exceeds the evidence, briefly flag that outside the draft and
  use accurate wording. Do not turn a prototype finding into production fact.
- Ask one consequential, answerable question adapted to what this person can
  help resolve. Include what their response would change. Do not manufacture
  a design solution or a rationale I have not supplied; ask if it is essential.
- Keep my actual question intact. Do not add a product/design/engineering
  question set, a reviewer map, a review packet, a new meeting, or a reminder.
- Return the message draft first, labeled with its intended person/channel.
  Add at most one brief check outside it if a missing link, access issue, or
  unsupported claim needs my attention. Do not send, post, tag, or schedule.
```

## Worked fictional example

All people, records, and behavior in this example are invented. There is no real issue or prototype link to open.

**Audience and channel:** Arun, the engineer responsible for delivery behavior, in the existing Slack thread for REL-42.

**Designer’s rough notes:**

> In the Relay prototype v0.4, 16 of 20 sends succeeded and four failed. The retry log shows another attempt to all 20 simulated recipients. I’m worried that in production, someone who already received the message could get it twice. My preference is to retry the failures. I don’t know whether production stores reliable per-recipient outcomes or can target only failed sends. I need Arun’s answer before choosing the recovery behavior.

**Evidence reference:** REL-42, prototype v0.4, retry log row 3. The observed behavior is in a simulation. Duplicate production delivery has not been observed.

**Draft for Arun in Slack:**

> Arun, in REL-42’s prototype v0.4, Retry attempts all 20 sends again after 16 succeed and four fail (retry log, row 3). I’m concerned that could mean duplicate messages in production. Can production reliably retry only the failed sends? I haven’t confirmed how per-recipient outcomes are stored; your answer will help me choose the recovery behavior.

Before using this with real work, replace the artifact reference with its actual link and confirm Arun can open it. Do not invent a permalink.

The request carries a position and a specific uncertainty. It does not claim that the backend supports failed-only retry, that customers received duplicates, or that a fix is approved. Arun can supply the relevant constraint, and the designer can use that answer in the next design choice.

### Adapt the question when the audience or decision changes

Keep the same facts and uncertainty. Change the request only when a different person’s input is needed.

- If a product owner is deciding scope, ask about the actual recovery tradeoff they need to resolve, including any still-unconfirmed engineering constraint. Do not quietly turn “Is failed-only retry possible?” into “Please approve a bigger redesign”
- If a leader is deciding investment, include the supplied consequence and the specific decision they own. Do not invent cost, customer impact, ROI, or urgency to make the request sound important
- If the recipient needs a technical detail, keep it. Brevity is useful only when the message still supports a useful answer

For a larger disagreement involving conflicting requirements, evidence, or several owners, use [01 Build a decision brief](Slide_12_Audit_Claims_Carry_Evidence_and_Build_a_Decision_Brief.md). This resource is the smaller step: ask the right person one useful question.

## Check the draft before using it

Read it once as the recipient. Can they tell what happened, where to look, what you need from them, and what their answer would change? Does it preserve your thinking and mark the real unknown? Correct any invented detail, check the artifact/version and access, then send it through your normal process.

When the answer changes the work, keep the useful constraint or decision beside the existing artifact or issue. A short exchange can be enough. Do not create another document or meeting just to satisfy this template.

## Keep it only if it helps

**“If it doesn’t work, dump it.”**

Try it on a few comparable real requests. Look at:

- **Preparation plus correction time:** Include gathering the input and fixing the AI’s draft, not just how fast it generates words
- **Response usefulness:** Did the person answer the consequential question with a usable fact, constraint, or decision?
- **Clarification loops:** Did you spend fewer exchanges explaining what you meant or finding the right artifact?
- **Decision movement:** Did the answer change a choice or resolve uncertainty? A reasoned confirmation of the current direction can be useful too

“Ten messages to three” is a goal to test, not a measured result or a promise. Fewer messages alone do not show better collaboration. If the draft takes as much correction as writing it yourself, hides an important uncertainty, or makes the exchange less useful, simplify the prompt or stop using it.

## Optional integration appendix

The prompt works without an integration. If your team later wants to route approved drafts into an existing tool, the separate [integration appendix](Slide_05_Optional_Review_Request_Integration_Guide.md) provides a small proposed record and safeguards. It is not required reading for writing a message and is not an installed workflow.

## Monday move

Choose one question you are already about to ask a colleague. Name the person and channel, give AI your rough concern and context, and ask for a brief request. Keep it only if the preparation, correction, and resulting exchange are better than your usual approach.
