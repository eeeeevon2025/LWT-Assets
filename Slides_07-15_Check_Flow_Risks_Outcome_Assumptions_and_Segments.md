Companion: 7 · Speed + Quality?; 15 · Remember to ask the right questions
Purpose: Review usability, the feature-to-outcome assumptions, and evidence about different users; or start with new-project questions.

# Ask the right questions and check a flow

## Run this resource on its own

1. Open an assistant approved by your organization for this material, such as an approved Cursor chat, Claude, or ChatGPT workspace. Use a read-only or drafting mode. No integration, installed command, or background automation is required or assumed.
2. Attach this complete Markdown file, or paste its entire text into the conversation. Then use the short invocation below. Alternatively, copy a complete prompt block from this file with your inputs; required templates are included in the relevant prompt.
3. Supply new-project question OR one existing flow; intended user/task and iteration purpose; artifact/version or documented steps/screenshots; approved PRD, intended business outcome/KPI, research, constraints and actual component references. For outcome and segment checks, include the proposed change, expected user behavior, and any approved segment-level findings or aggregate reports. Give each report its segment definition, event/metric meaning, counts and denominators, time window, and known sampling or coverage limits; label anything unavailable. Attach approved files or paste labeled excerpts with source names, dates and locations. A link is usable only if the assistant can actually read it. Redact personal or restricted details under your organization's rules; never include credentials.
4. Ask it to list what it could inspect before drawing conclusions. If essential inputs are missing, keep the output provisional and ask for the smallest useful evidence or access request. Missing evidence is not a finding.
5. Expect up to three consequential questions for a new project OR up to five source-linked candidate findings for an existing flow, with consequences and the next human check. For a feature review, include the change → behavior → business-result chain and a brief segment-evidence check; use these to select the same capped findings, not extra lists of speculative defects. Check important claims against their sources and confirm decisions with the relevant people before using the draft.

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
Slides 15, “Remember to ask the right questions,” and 16, “My working system for design”

**Monday move:** On a new project, ask the question that could change what you build. For existing work, check one flow against its intended behavior.

## Try the approach

Choose the route that matches the work. For a **new project**, use the questions prompt below with the context you have; a finished artifact is not required. For **existing work**, compare the current artifact with its intended behavior. In either case, ask AI to prepare specific questions and evidence while choices are still open, then have the right people judge the consequences.

The talk's separate existing-work example is **UXCartographer**. Yvonne describes it as using project knowledge placed in a Cursor folder to analyze gaps and divergence from a PRD. Her separate short recording will show the app's actual behavior; this description is not an independent code inspection.

You can try either portable prompt below with approved material without using the app. The wider check menu describes possible review work, not features verified in UXCartographer. This first-pass aid cannot certify accessibility, establish user value, validate security, or authorize release. A Markdown download does not install a command, connect a tool, or run a test.

## New project questions prompt

> Help me find the next consequential UX question for [project or idea], using only [approved context and sources]. A prototype may not exist yet. Start with what you can actually read. Separate observed evidence, interpretations, repeated claims, and unknowns; cite the relevant source or say that evidence is missing.
>
> Consider who is trying to do what, the change we want, assumptions about the need, important states and recovery, and what someone must understand or verify before a consequential action. Choose only the questions relevant to this project. Return at most three unanswered questions, why each could change the next decision, and the smallest evidence check or relevant expertise needed. Then ask me the single most consequential question first and wait for my answer.
>
> Do not treat a proposed solution as an established need or invent users, requirements, feasibility, owners, or findings about an artifact you have not inspected. Stay read-only and stop for my review; do not build, post, contact anyone, or approve scope.

Use [resource 05](Slide_11_Build_a_Shared_Context_Brief.md) first if you need a linked context brief. Keep the answer in the existing working record; a question does not need a separate document by default.

## Existing work review

1. Pick one flow and its intended person/task. State what this iteration is for: learning, a demonstration, or a release assessment
2. Supply the artifact/version and the PRD, project knowledge, research, decisions, or constraints the assistant may read. State the proposed change, expected user behavior, and intended business result/KPI separately. Add approved segment-level evidence with definitions, counts/denominators, time windows, and limitations when available. A rough artifact can come first; its code does not establish approved purpose, and a PRD records an intention rather than proving it will work
3. List actual access and gaps. Use questions-only mode if the artifact cannot be inspected. Pasted excerpts or selected screenshots/code are valid inputs, with corresponding limits
4. Review the few findings that could change the next decision. Have the relevant person confirm severity, scope, and any changes

Use existing authorized tools. If an issue connector, design system, runtime, or test result is unavailable, say so. Do not broaden access merely to complete a checklist or ask the author to re-enter facts already available.

### Artifact review prompt

> Review [artifact/version and one flow] for [intended person and task], using only [approved PRD, project knowledge, and other sources]. This iteration is for [purpose; unknown is acceptable]. Draft findings for my review.
>
> First state what you can actually read and inspect, what is simulated, and what is missing. If needed, ask the single most consequential question. Compare intended behavior with what the material shows. Keep observations, inferences, contradictions, and unknowns distinct; cite exact sources or artifact locations.
>
> Select relevant checks: outcome assumptions, people hidden by averages, states and recovery, clear actions, content, actual supplied design-system use, accessibility, and prototype honesty. For a feature review, first draft two compact evidence maps:
>
> 1. Proposed change → expected user behavior → business result/KPI. For each link, list its source and status: directly observed association, inferred explanation, assumption, contradictory evidence, or unknown. Say what the source actually supports; an association does not establish causation, and a target in a PRD is not evidence. Identify the weakest consequential link and the smallest research question or comparison that could change the scope decision. Do not invent experiment results, feasibility, or causal effects.
>
> 2. Segment-evidence check. Use only supplied, approved segment definitions/findings to examine whether the same design could help one group but hinder another. For supported comparisons, show metric/event definitions, counts and denominators, time window, exposure and known coverage limits. If these are absent or incomparable, explain the limitation and draft the precise data request or user-research question. Label possible differences as hypotheses, not segment findings. Do not invent personas, synthetic users, demographics, segment behavior, or statistical significance; do not infer individual traits from group averages.
>
> Use both maps to choose at most five consequential findings in total across all checks. Do not add separate uncapped finding lists. For each: evidence/location, observed defect or candidate concern, affected person/task and possible consequence, confidence or missing information, the smallest next check, and the expertise needed to validate it. Suggest priorities for human confirmation; do not give a blanket usability or accessibility score.
>
> Do not claim a test ran unless you actually ran it and can give its method and result. State which questions require manual/runtime checks. End with one harder design question worth attention after routine checks, the smallest next step, and evidence that would change the assessment.
>
> Stay read-only. Do not edit files, execute scripts, install packages, post findings, contact people, create reminders, or approve release. Name owners only when documented; otherwise identify the expertise needed. Stop for my review.

## Choose the relevant checks

Use this menu inside the workflow. Select only what could affect the task or decision.

| Area | AI can help inspect or prepare | A person still needs to validate |
| --- | --- | --- |
| Outcome assumptions | Map proposed change → expected user behavior → business result; locate support, contradictions, and untested links in supplied sources | Whether the goal and mechanism make sense, what evidence is strong enough, and which comparison could change the decision |
| People hidden by averages | Organize approved segment findings and identify missing comparison evidence | Whether groups, measures, exposure, and samples are comparable; whether a suspected benefit or burden occurs in real use |
| State coverage | Relevant empty, loading, success, partial-success, error, permission, interruption, and recovery states | Which states matter and whether the actual interaction supports recovery |
| Clear actions | Ambiguous names, feedback, and resulting states | Whether people understand the language and it matches real behavior |
| Design-system use | Components and tokens against the actual supplied system | Whether deviations are intentional and correctly implemented; no supplied system means no compliance claim |
| Content | Missing instructions, unexplained terms, inconsistent labels | Domain accuracy, context, and the consequence of misunderstanding |
| Accessibility | Available markup, candidate keyboard/assistive-technology checks, and supplied test results | Real behavior, semantics, meaningful alternatives, and barriers automated checks miss |
| Prototype honesty | Mock data, hard-coded success, unsupported controls, and unimplemented consequences | Whether reviewers can tell what is real and what this iteration can answer |

### Expose the assumption between the feature and the outcome

Ask AI to map **proposed change → expected user behavior → business result**, then label the evidence and assumptions at each link. This is a check on the feature's rationale as well as its interaction details. Agree the relevant user goal and business objective with the team; do not assume the PRD has already established either the need or the mechanism.

**Fictional example, not a finding about your project:** “Scratch interaction → more interest → more purchases” contains several bets. If supplied research shows shoppers cannot tell which products qualify, UX can propose comparing clearer eligibility with the interactive treatment before committing to a larger build. AI can assemble the source-backed rationale, draft the alternatives, and suggest what to ask or measure. People confirm the research design, implementation effort, and decision.

Keep the alternatives comparable: say what remains the same, such as the offer and intended audience, and what changes. A usability comparison might reveal comprehension or task problems; it does not by itself prove an effect on purchases. Ask the data or experimentation team what would be needed for that claim.

### Look for people hidden by the average

Give AI approved segment-level findings and ask: **Where might the same design help one group and hinder another, and what evidence would let us tell?** Use existing research segments or task contexts; do not manufacture groups because a comparison sounds plausible.

**Hypothesis to investigate, not a known difference:** A playful reveal might appeal to browsers and slow repeat buyers who know what they want. Ask AI to locate any supplied support or contradiction and, if none exists, draft a request for evidence. For example: “Can we compare task completion, time and errors for these documented task contexts, with each group's definition, exposure, counts/denominators, date window, and instrumentation limits?” Ask users how they found, understood, and redeemed the offer without suggesting that the reveal must have helped or hindered them.

Do not create user-level profiles or upload restricted records. Use approved aggregate evidence and retain small-sample/privacy restrictions. Aggregate differences can reflect traffic mix, eligibility, exposure, or measurement differences; flag these explanations rather than declaring that the design caused a difference. A missing segment breakdown is an evidence gap, not proof of harm.

### State and recovery questions

- Can someone tell whether an action saved, submitted, activated, or only previewed something?
- What do empty, loading, partial, stale, and denied-permission states help them do next?
- Are inputs preserved after a recoverable failure? Can someone correct, cancel, go back, or get help?
- Could repetition create duplicate work, invitations, messages, or transactions?
- If completion is uncertain, does the interface preserve that uncertainty?
- What should someone verify before an irreversible or high-consequence action?

These are questions to investigate, not proof that the system has each failure mode.

### A preliminary accessibility pass

Consider titles, headings, image/media alternatives, meaningful control names, field labels and errors, keyboard operation, visible focus, contrast and non-color cues, text resizing and narrow layouts, dynamic status, and relevant motion or time limits.

A screenshot cannot establish keyboard or screen-reader behavior. A code excerpt does not establish full rendered behavior. A clean automated scan cannot establish that an experience is accessible. Keep actual results separate from proposed manual checks; involve appropriate expertise and, where useful, people with disabilities.

[W3C WAI Easy Checks](https://www.w3.org/WAI/test-evaluate/preliminary/) covers a preliminary review, not a complete evaluation. [Selecting Evaluation Tools](https://www.w3.org/WAI/test-evaluate/tools/selecting/) explains tools' role and limits. References checked October 2, 2026. This aid is not certification or legal advice.

## Make the prototype inspectable

When someone else needs to try a code prototype, check for:

- Verified start/reset steps, without secrets or hidden live consequences
- Fictional fixtures and explicit persistence, mock, and simulated-integration boundaries
- Safe ways to reach relevant empty, failed, partial-success, and recovery states
- Understandable states and an explanation of what remains unimplemented
- An honest record of what was inspected, tested, failed, or left untested

Do not execute unfamiliar commands or install dependencies under this prompt. Running checks or changing code is a separate authorized step. A usable prototype still needs engineering review before it becomes a production commitment.

## Keep the result small

Return artifact/version, iteration purpose, actual source coverage, and, for a feature review, a compact outcome chain and segment-evidence check. Then return at most five prioritized findings across all checks and one focused next question. Label unsupported candidate concerns as hypotheses or evidence requests, rather than established findings. Keep each finding's evidence, uncertainty, consequence, next check, and human-validation need together.

For a quick fictional example, a bulk-invite prototype always displays “20 invitations sent.” The selected code shows a fixed success string, with no request or mixed-result state. AI can identify that simulation and propose a scenario to inspect. It cannot conclude that production delivery, retries, or accessibility fail. The deeper question is what someone needs to know and do when only some invitations succeed.

Use [resource 01](Slide_12_Audit_Claims_Carry_Evidence_and_Build_a_Decision_Brief.md) if a consequential finding needs a source audit or shared decision brief. Use [resource 08](Slide_05_No_Handoff_Prepare_a_Useful_Review_Request.md) when one colleague's expertise would resolve the question. Do not turn every first-pass concern into a large review packet.

## Pick one Monday experiment

1. List unrepresented recovery states in a flow you are already building
2. Compare one generated screen with the actual design system and review the differences
3. Use an approved automated accessibility check, then manually inspect the task it cannot evaluate
4. Ask a colleague to complete one non-happy-path task without your narration
5. Map one feature’s proposed change → behavior → business result and investigate its weakest assumption
6. Check whether an average hides a consequential difference in approved segment evidence, or draft the missing evidence request
7. If drafting time is genuinely recovered, compare two different solutions to the hard problem

Record the routine task, AI time, review/correction time, what you used any remaining time for, and whether it changed a decision. Estimated savings are not a performance claim.

The check menu and experiments formerly in resource 04 are now part of this workflow. The earlier standalone draft is not included in this download.
