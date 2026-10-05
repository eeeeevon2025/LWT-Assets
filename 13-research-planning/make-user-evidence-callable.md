# Make User Evidence Callable

AI can make an idea look finished before the evidence is.

This resource helps teams connect the work they are building to the customer evidence their organization already has, so anyone on the team can ask:

> **What do we actually know about this?**

The goal is not to create another research repository or another giant prompt. It is to make existing user evidence easier to reach from the work itself.

---

## 1. Connect the evidence you already have

Give your AI workspace access to the customer-evidence sources your organization already uses, where permissions allow.

These might include:

- User research repositories
- Customer support conversations
- Interview transcripts
- Sales or customer-success calls
- Surveys and feedback
- Product analytics
- Research docs in Drive, Notion, Confluence, or similar tools
- CRM or customer records

Depending on your environment, that connection may happen through a built-in connector, API, MCP server, enterprise search, or retrieval layer.

**Do not copy everything into one giant prompt if the AI can retrieve the original source instead.**

---

## 2. Create a shared `@user-evidence` skill

Use the following instruction as a shared AI skill, agent instruction, project instruction, or reusable prompt.

```text
# USER EVIDENCE

You are the evidence layer for this product team.

When I ask a question about a feature, requirement, design, customer problem, or product decision, search the connected customer-support and user-research sources for relevant evidence.

Your job is not to make the case for the work.
Your job is to tell us what the evidence actually supports.

For every response:

1. Show the strongest relevant evidence.
   Include the original source, date, customer/user segment, and link when available.

2. Separate observation from interpretation.
   Clearly distinguish what users actually said or did from what the team or AI is inferring.

3. Do not inflate confidence.
   If evidence is limited, old, indirect, contradictory, or based on a small sample, say so.

4. Look for disagreement.
   Surface evidence that contradicts the dominant interpretation, not just evidence that supports it.

5. Do not turn frequency into causality.
   A commonly reported issue is not automatically the cause of a behavior or business outcome.

6. Do not invent evidence.
   If the available sources cannot answer the question, say:
   "We don't know from the evidence available."

7. Return the source.
   Make it easy for a human to open the original research, transcript, ticket, call, or data source.

When useful, organize the response as:

WHAT WE KNOW
Evidence directly supported by available sources.

WHAT WE SUSPECT
Reasonable interpretations that have not been established.

WHAT CONFLICTS
Evidence pointing in another direction.

WHAT WE DON'T KNOW
Important unanswered questions.

SOURCES
Original evidence used.
```

---

## 3. Call it from the work

### Before designing

```text
@user-evidence What do we know about the problem this feature is supposed to solve?
```

### Reviewing a prototype

```text
@user-evidence Compare this flow with what users have actually told us.
Where are we making assumptions?
```

### Writing requirements

```text
@user-evidence What evidence supports these requirements?
Flag any requirement that appears to be based mainly on inference.
```

### Engineering

```text
@user-evidence Why are we building this behavior?
Show me the customer evidence behind the decision.
```

### Challenging a direction

```text
@user-evidence Find evidence that contradicts our current approach.
```

### Checking certainty

```text
@user-evidence What are we treating as known here that the evidence only supports as a hypothesis?
```

---

## 4. Design principle

### Polish outruns proof.

AI makes it incredibly easy to turn a hypothesis into a convincing artifact.

A polished prototype, specification, or implementation can create the feeling that a decision is settled even when the evidence underneath it has not changed.

So do not only make the work easier to generate.

**Make the evidence easier to reach.**

The goal is to make it harder for:

> **"We suspect..."**

to quietly become:

> **"We know..."**

just because the artifact looks finished.

---

## 5. Guardrails

A useful evidence skill should:

- Cite or link back to original sources whenever possible
- Distinguish direct evidence from interpretation
- Preserve dates, sample size, and user segment when available
- Surface conflicting evidence
- Say when evidence is weak or missing
- Avoid turning a few quotes into a population-level claim
- Avoid turning correlation into causation
- Avoid inventing user needs from product requirements
- Keep sensitive customer data inside the organization's approved access controls

The AI should help people **find and interrogate evidence**, not replace researchers or human judgment.

---

## 6. Implementation options

The exact implementation will depend on your stack.

Possible patterns include:

- A shared project instruction connected to research files
- A reusable AI skill or agent
- An MCP server exposing approved research sources
- Retrieval over support tickets or research transcripts
- Enterprise search across research, support, CRM, and product docs
- A command or mention such as `@user-evidence` inside an internal AI workspace

The interface matters less than the behavior:

> Anyone doing the work should be able to ask what users actually told us without leaving the context of the work.

---

## A useful test

If an engineer, designer, PM, or researcher is looking at a polished feature and asks:

> **Why are we doing this?**

Can they get from the artifact to the original user evidence in seconds?

If not, the evidence is still too far away from the work.

---

## The idea in one line

**Connect the work to the evidence. Make user proof callable.**
