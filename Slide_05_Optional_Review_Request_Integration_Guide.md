Companion: 5 · There is no handoff · optional integration proposal
Purpose: Team-configured review workflow proposal; downloading does not install or run it.

# Optional routing for a useful review request

## Use this appendix on its own

Open an approved assistant in drafting mode. Paste the complete prompt below with an already reviewed message draft, intended person/channel, approved artifact reference/version, and your organization's sending-approval requirements. Include available integration documentation only if it is approved for this assistant. No connector is required to draft the plan. This appendix does not implement routing or send the request.

```text
Draft a field map and safety checklist for routing ONE review request.
Reviewed draft: [paste]
Intended person and existing destination: [supply verified details or unknown]
Artifact reference/version and permitted audience: [supply]
Approval requirements and available tool documentation: [supply or unknown]

Return a draft record with: request ID, author, verified recipient, channel,
verified destination, artifact reference/version, one consequential question,
message draft, approval status, approved-content reference, sent-message ID,
and delivery status. Use unknown/null for unverified values, draft for approval
status, and not sent for delivery status; do not invent identifiers or receipts.
List missing confirmations: identity, destination visibility, artifact access,
actual tool capability, and exact content/recipient approval. Keep a failed or
uncertain send distinct from confirmed delivery; propose verification before
retrying. Describe the smallest manual alternative if access is missing.
Return only a proposed record and checklist for a person to review. Do not
configure tools, install integrations, change permissions, send/edit messages,
subscribe anyone, or create monitoring or reminders.
```

Expected result: a proposed field map, unresolved confirmations, and a manual fallback. The example record below is a reference, not an API schema or proof of compatibility.


LWT Field Kit · Companion to 08 Prepare a useful review request · October 2, 2026

Use this only if your team chooses to connect the drafting step to an existing communication or issue tool. The basic prompt needs no integration. This is a proposed field map, not an API schema, executable code, installed connection, or claim of native platform support.

Keep one draft for the intended person and existing conversation. A simple record could contain:

```json
{
  "request_id": "stable identifier for this request",
  "author": "verified author",
  "recipient": "verified intended person",
  "channel": "the approved communication channel",
  "destination": "verified existing conversation or issue",
  "artifact_reference": "authorized source link",
  "artifact_version": "version or date",
  "question": "one consequential question",
  "draft": "author-reviewed message text",
  "approval_status": "draft",
  "approved_content_reference": null,
  "sent_message_id": null,
  "delivery_status": "not sent"
}
```

Verify actual tool capabilities and permissions before implementing any routing. Review these safeguards with whoever configures it:

- Resolve the correct recipient and destination. A named role, issue assignee, channel member, or prior commenter does not automatically become a recipient
- Check who can see the destination and whether the intended person can open the artifact. Do not expand access, add recipients, or change subscriptions merely to make delivery work
- Keep drafting separate from permission to send. Follow the organization’s approval rules and retain the approved content and recipient scope. Do not infer permission from this example record
- Preserve the author’s concern and uncertainty when adapting the wording. Flag unsupported claims before sending rather than making them more persuasive
- Check whether a prior send succeeded before retrying an uncertain result. Retain its verified message ID; do not create duplicate posts because a confirmation was missing
- If an update is needed, read the latest message or comment first. Edit only content the workflow owns and is authorized to change; do not overwrite a human’s contribution
- Stop when the approved request is delivered or delivery requires the author’s help. Do not add reminders, reply monitoring, meetings, tasks, or broader reviewer groups without a separate request and appropriate authorization

If the integration adds more setup or correction work than it removes, use the prompt manually in the existing conversation. A saved Markdown file has no background routing behavior.
