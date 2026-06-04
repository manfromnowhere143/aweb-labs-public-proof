# Aweb Technical Reviewer Guide

This guide is for technical reviewers, infrastructure investors, startup programs, and design partners who want to understand Aweb quickly without reading private implementation details.

## The Core Claim

Aweb is Mission Control Cloud for governed AI agent work.

The product is not another model interface. It is the operating layer around agents that touch real tools: intent capture, capability routing, policy, approval gates, execution, validation, receipts, and recovery.

## What To Review First

| Step | Artifact | What to check |
| --- | --- | --- |
| 1 | [README.md](./README.md) | Positioning, public proof surface, product boundary. |
| 2 | [SPEC.md](./SPEC.md) | Governed run state machine, manifest shape, receipt shape, boundary classes. |
| 3 | [PUBLIC-PROOF.json](./PUBLIC-PROOF.json) | Machine-readable index of public surfaces, claims, and boundaries. |
| 4 | [examples/funding-ops-run.manifest.json](./examples/funding-ops-run.manifest.json) | Example run manifest for a high-consequence founder workflow. |
| 5 | [examples/funding-ops-receipt.redacted.json](./examples/funding-ops-receipt.redacted.json) | Redacted receipt showing blocked external actions and safety checks. |
| 6 | https://aweblabs.ai/agent-operations-audit | Commercial intake for one real workflow audit. |

## Engineering Questions Aweb Is Built To Answer

- What exactly did the human ask the agent system to do?
- Which tools, APIs, MCP capabilities, providers, or data systems were in scope?
- Which policy class applied to each action?
- Which actions were read-only, local-write, externally gated, secret-gated, or claim-gated?
- What evidence was used before execution?
- What did the system refuse to do?
- What did the human approve?
- What changed, what failed, and what remains unresolved?
- Can the run be reviewed or repeated without relying on chat history?

## Non-Negotiable Invariants

These are the standards Aweb is trying to make boring and inspectable:

| Invariant | Meaning |
| --- | --- |
| Default-deny external action | Email, submit, post, payment, account, legal, credential, and financial actions require explicit human approval. |
| No secret leakage | Credentials, OAuth tokens, private inbox contents, legal docs, wallet instructions, and private investor/customer data do not belong in public proof. |
| Evidence before action | High-consequence actions should carry source maps, claim checks, and receipt evidence. |
| Receipts after action | Completed, blocked, failed, and rejected runs should leave a durable summary of what happened. |
| Honest uncertainty | Missing source material, stale claims, duplicate risk, and incomplete setup should block or downgrade the run instead of being hidden. |
| Finance boundary | GEX and Veritas are framed as research, simulation, risk visibility, and decision support; not investment advice or autonomous capital deployment. |

## What This Repo Proves

- Aweb has a clear public thesis around governed agent execution.
- The company is dogfooding the operating loop for its own high-consequence workflows.
- The public proof model has explicit manifest, state, receipt, and boundary language.
- The commercial entry point is narrow enough to be bought and reviewed: one Agent Operations Audit for one real workflow.
- The public surface avoids private source code, credentials, internal logs, legal documents, and unverifiable traction claims.

## What This Repo Does Not Claim

- It is not a complete source release of Aweb.
- It is not a security certification.
- It is not a customer-traction claim.
- It is not a financial product, trading promise, or investment offer.
- It does not authorize anyone to send emails, submit forms, deploy systems, charge payments, or publish private details without Daniel's approval.

## High-Signal Review Path

If you have 10 minutes:

1. Read the first screen of [README.md](./README.md).
2. Inspect the state machine and boundary classes in [SPEC.md](./SPEC.md).
3. Compare the example manifest and receipt in [`examples/`](./examples).
4. Check that public links resolve under `https://aweblabs.ai`.
5. Ask one question: "Where would this system stop before doing something risky?"

If that question has a crisp answer, the control-plane thesis is working.

## Best Next Conversation

The best practical next step is a focused review of one real workflow:

- one agent or internal operation,
- one tool/API/MCP path,
- one approval boundary,
- one receipt model,
- one implementation roadmap.

Public intake: https://aweblabs.ai/agent-operations-audit

Contact: business@aweblabs.ai
