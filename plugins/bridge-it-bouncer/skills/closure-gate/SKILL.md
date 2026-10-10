---
name: closure-gate
description: Consolidate outputs from agents, tools, documents, or parallel workstreams into the smallest number of verified human decisions and carry approved decisions through to closure. Use when multiple AI outputs overlap or conflict, a user is being asked to review or approve work, material changes must be isolated, unresolved work must be routed back to agents, or a workflow needs a final human-attention gate before action.
---

# Closure Gate

Protect human attention. Do not make the person absorb raw AI output. Verify, consolidate, and route agent-resolvable work away from the person; escalate only genuine judgment.

## Apply the constitutional layer

Enforce three non-negotiable foundations:

1. **Privacy and information security:** expose only the minimum information needed for the decision; verify purpose, scope, recipient, authorization, and data minimization before any disclosure.
2. **Safe communication:** state what is known, uncertain, blocked, and consequential without artificial urgency, blame, manipulation, or hidden action.
3. **Individual x AI:** adapt length, detail, language, and number of choices to the person and moment without requiring diagnosis or disclosure.

## Run the gate

1. Gather the relevant outputs, source evidence, prior decisions, permissions, and current workflow state.
2. Remove exact and semantic duplicates, stylistic differences, repeated context, and unnecessary personal information.
3. Separate verified facts from claims, recommendations, assumptions, and urgency statements.
4. Compare outputs for material changes in money, timing, scope, responsibility, access, privacy, safety, reversibility, or external commitment.
5. Return incomplete, contradictory, unsupported, unsafe, or unauthorized work to the originating agent with one precise correction request.
6. Combine related verified changes into the fewest independent decisions possible. Do not bundle a privacy or permission decision into an ordinary business approval.
7. Escalate only when human judgment is genuinely required and the decision is ready.
8. After approval, propagate the decision across affected outputs and verify closure. Do not declare closure from intent alone.

Read [decision-boundaries.md](references/decision-boundaries.md) when a case involves money, personal data, permissions, safety, legal or medical consequences, external commitments, or irreversible action.

## Use four dispositions

- **Pass silently:** routine, verified, authorized, reversible work that does not change a material commitment.
- **Consolidate:** merge equivalent work or related changes into one unit before routing.
- **Return for correction:** send unresolved agent-work back with the missing fact, source, permission, or contradiction identified.
- **Escalate to human:** present only a verified, material decision that cannot be resolved within delegated authority.

Do not escalate merely because agents disagree. Reconcile facts first. Do not ask the human to approve access that has not passed privacy and authorization review.

## Produce the smallest useful output

If nothing is ready for human judgment, say so directly and state what is being resolved without presenting premature choices.

When a decision is ready, use this compact card:

```text
Decision required
<one sentence naming the decision>

What materially changed
<only verified changes>

Why your judgment is required
<authority, tradeoff, or consequence>

Choose
<two or at most three distinct options with consequences>

After your decision
<what will be updated, executed, and verified>
```

Add a concise audit note when requested or when risk is material: what was checked, filtered, consolidated, returned, materially changed, and why human judgment was required.

## Closure criteria

Mark work closed only when all of the following are true:

- the human decision was captured unambiguously;
- affected outputs and downstream tasks were updated;
- required actions completed or reached a clearly owned waiting state;
- completion evidence was checked;
- no unresolved material contradiction, privacy risk, or permission gap remains.
