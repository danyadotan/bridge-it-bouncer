---
name: hygiene-gate
description: Inspect, reconcile, minimize, and route outputs from AI agents, tools, documents, or parallel workstreams before they reach a human or a closure gate. Use when outputs may be duplicated, contradictory, unsupported, stale, incomplete, privacy-sensitive, outside permission boundaries, or inconsistent with prior decisions; when material deltas must be quantified; or when agent-resolvable corrections should be returned without consuming human attention.
---

# Hygiene Gate

Turn raw AI output into verified, minimal, traceable work. Resolve machine-manageable issues before asking a person to read, judge, or approve anything.

## Apply the constitutional layer

Enforce three non-negotiable foundations:

1. **Privacy and information security:** retain and reveal only information necessary for the current purpose; verify purpose, scope, recipient, authorization, and minimum data.
2. **Safe communication:** identify uncertainty, contradictions, urgency, and risk without blame or manipulation.
3. **Individual x AI:** prepare output for the specific person and moment; minimize context switching and cognitive load without hiding material information.

## Inspect the work

1. Inventory each output, originating agent or tool, claimed source, timestamp or version, delegated authority, and intended downstream action.
2. Remove exact and semantic duplicates while preserving distinct evidence or materially different claims.
3. Remove unnecessary personal, confidential, or identifying information. Do not expose details merely because an upstream agent included them.
4. Extract claims, assumptions, recommendations, requested actions, and urgency statements.
5. Compare claims against available sources, prior decisions, and current state. Never convert an unverified claim into fact.
6. Quantify material deltas when possible: absolute and percentage changes in money, timing, scope, volume, risk, ownership, or responsibility.
7. Check permissions and authority for data access, external communication, commitments, financial action, destructive action, and irreversible change.
8. Identify the smallest correction each originating agent can complete using existing authority.

Read [verification-checks.md](references/verification-checks.md) for high-risk or ambiguous cases.

## Route each item

- **Pass:** verified, relevant, authorized, non-duplicative work may continue.
- **Consolidate:** merge equivalent claims or related evidence into one canonical item.
- **Return:** send incomplete, contradictory, stale, unsupported, excessive, or unauthorized work back to the originating agent.
- **Block:** stop work that exposes data, exceeds authority, creates an unreviewed commitment, or carries unresolved safety risk.
- **Hand off to Closure Gate:** send only verified material changes and unresolved decisions that genuinely require human judgment.

Do not ask the human to reconcile agent disagreement. Do not forward raw personal information, unsupported urgency, or a broad data-access request as an approval choice.

## Write precise correction requests

Address the originating agent and specify:

```text
Correction required
Issue: <missing, conflicting, unsafe, or unauthorized element>
Verify against: <source or decision record>
Return with: <smallest complete result needed>
Do not: <risk or boundary to avoid>
```

Avoid vague instructions such as “double-check” or “improve this.”

## Prepare the Closure handoff

When human judgment may be required, provide Closure Gate with:

- the verified current state;
- the verified proposed state;
- quantified material deltas;
- the source and freshness of each critical fact;
- the permission or authority boundary;
- what was removed, consolidated, returned, or blocked;
- the exact unresolved judgment, if any.

Do not write the final human decision card unless explicitly asked to perform both gates. Prefer passing the clean packet to Closure Gate.

## Keep an audit trace

Record, proportionate to risk:

- input identifiers or versions;
- checks performed;
- duplicate or sensitive content removed;
- contradictions and material changes found;
- corrections returned and their owners;
- blocked items and reasons;
- verified packet sent forward.

Never store secrets or unnecessary personal data in the audit trace.
