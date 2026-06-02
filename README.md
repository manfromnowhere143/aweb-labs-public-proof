<p align="center">
  <a href="https://aweb-wine.vercel.app/final">
    <img src="https://aweb-wine.vercel.app/identity/aweb-business-mail-avatar.png" width="104" alt="Aweb avatar">
  </a>
</p>

<h1 align="center">Aweb Labs Public Proof</h1>

<p align="center">
  <strong>Mission Control Cloud for governed AI agent work.</strong>
</p>

<p align="center">
  <a href="https://aweb-wine.vercel.app/final">Final</a>
  &nbsp;/&nbsp;
  <a href="https://aweb-wine.vercel.app/v2">V2</a>
  &nbsp;/&nbsp;
  <a href="https://aweb-wine.vercel.app/product">Product</a>
  &nbsp;/&nbsp;
  <a href="https://aweb-wine.vercel.app/docs">Docs</a>
  &nbsp;/&nbsp;
  <a href="https://aweb-wine.vercel.app/docs/mcp">MCP</a>
  &nbsp;/&nbsp;
  <a href="https://aweb-wine.vercel.app/docs/api-reference">API</a>
  &nbsp;/&nbsp;
  <a href="./SPEC.md">Spec</a>
  &nbsp;/&nbsp;
  <a href="./COLLABORATION.md">Collaboration</a>
</p>

---

Aweb connects AI models, APIs, MCP tools, provider warehouses, databases, governed execution, code validation, approvals, and system builders into auditable AI production workflows.

This repository is the public proof surface for reviewers, investors, collaborators, grant programs, and startup programs. It is deliberately safe: no private source code, credentials, customer data, investor communications, internal logs, application links, legal documents, or wallet instructions.

The short version:

> Let agents do ambitious work. Make the boundary boring, explicit, and inspectable.

## Aweb In One Screen

| Question | Answer |
| --- | --- |
| What is Aweb? | Mission Control Cloud for governed AI agent work. |
| What does it connect? | Models, APIs, MCP tools, provider catalogs, databases, execution environments, approvals, and system builders. |
| What is the product category? | Agentic orchestration, governed execution, AI operations, and control-plane infrastructure. |
| What is the proof? | Aweb is using the same operating loop to run its own communication, application, funding, and material-preparation workflows under Daniel's approval. |
| Who is building it? | Daniel Wahnich, founder/operator, Israel. |
| What is it not? | Not a chatbot wrapper, not a website builder, not a Web3-first pitch, not a trading-profit product. |

## Reviewer Path

| Step | Surface | Why it matters |
| --- | --- | --- |
| 1 | https://aweb-wine.vercel.app/final | Current public positioning, founder proof, live product links. |
| 2 | https://aweb-wine.vercel.app/v2 | Current application surface and operator direction. |
| 3 | https://aweb-wine.vercel.app/product | Product framing for governed agent workflows. |
| 4 | https://aweb-wine.vercel.app/docs | Public docs and architecture entry point. |
| 5 | https://aweb-wine.vercel.app/docs/mcp | MCP/tool integration direction. |
| 6 | https://aweb-wine.vercel.app/docs/api-reference | API-facing platform surface. |
| 7 | https://aweb-wine.vercel.app/api-warehouse/providers | Provider and capability discovery surface. |
| 8 | [SPEC.md](./SPEC.md) | Public control-plane manifest and receipt shape. |

## Control Plane

```mermaid
%%{init: {"theme": "base", "themeVariables": {"primaryColor": "#111111", "primaryTextColor": "#ffffff", "primaryBorderColor": "#111111", "lineColor": "#555555", "secondaryColor": "#f5f5f5", "tertiaryColor": "#ffffff"}}}%%
flowchart LR
  Operator["Human operator / team"] --> Mission["Mission Control Cloud"]

  subgraph Orchestration["Aweb operating layer"]
    Mission --> Maestro["Maestro"]
    Maestro --> Policy["OS9 / Trust Runtime"]
    Policy --> Approvals["Approval gates"]
    Policy --> Validation["Validation"]
    Policy --> Receipts["Receipts and evidence"]
  end

  subgraph Capability["Capability fabric"]
    Maestro --> API["API Warehouse"]
    Maestro --> MCP["MCP Warehouse"]
    Maestro --> Code["Aweb Code"]
    Maestro --> Memory["Databases / memory"]
  end

  subgraph World["External work"]
    API --> Providers["Provider APIs"]
    MCP --> Tools["MCP tools"]
    Code --> Execution["Governed execution"]
    Memory --> State["State and context"]
  end

  Receipts --> Audit["Audit / debug / repeat"]

  classDef dark fill:#111111,stroke:#111111,color:#ffffff;
  classDef light fill:#f6f6f6,stroke:#cfcfcf,color:#111111;
  class Mission,Maestro,Policy dark;
  class Operator,Approvals,Validation,Receipts,API,MCP,Code,Memory,Providers,Tools,Execution,State,Audit light;
```

The model can improvise. The control plane should not.

Aweb's job is to keep agent work routed, bounded, approved, validated, evidenced, and repeatable.

## Operating Loop

```mermaid
sequenceDiagram
  participant D as Daniel / operator
  participant A as Aweb Mission Control
  participant S as Scout and recover
  participant M as Materials source map
  participant G as Approval gate
  participant X as External route
  participant R as Receipt / ledger

  D->>A: Set objective, constraints, and risk boundaries
  A->>S: Search, recover context, and dedupe prior actions
  S->>R: Record what exists, what is stale, and what is blocked
  A->>M: Select current public-safe source material
  M->>G: Prepare exact draft or field map
  G->>D: Stop for approval before send, submit, or post
  D->>X: Approve final external action
  X->>R: Store result, response, and follow-up state
```

This loop is not a demo script. It is how Aweb is operating its own serious workflows.

## Product Surface

```mermaid
flowchart TB
  Core["Aweb core"]

  Core --> Mission["Mission Control Cloud"]
  Core --> Maestro["Maestro"]
  Core --> Warehouse["API + MCP Warehouse"]
  Core --> Trust["OS9 / Trust Runtime"]
  Core --> Receipts["Agent Receipts"]
  Core --> Code["Aweb Code"]
  Core --> Builders["System builders"]

  Builders --> GEX["GEX"]
  Builders --> Veritas["Veritas"]
  Builders --> Nina["Nina"]
  Builders --> Leony["Leony"]

  GEX --> GEXNote["Research-grade market analytics"]
  Veritas --> VeritasNote["Probability and calibration research"]
  Nina --> NinaNote["Creative revenue operations"]
  Leony --> LeonyNote["AI creative studio workflows"]
```

Core components:

- **Mission Control Cloud:** the operator surface for governed agent work.
- **Maestro:** orchestration for durable multi-step workflows.
- **API Warehouse:** provider API capability mapping and generated client direction.
- **MCP Warehouse:** tool/provider discovery and adapter surface.
- **OS9 / Trust Runtime:** approvals, policies, boundaries, and evidence.
- **Aweb Code:** validation and governed execution path.
- **System builders:** vertical products and workflow surfaces built on the same substrate.

Vertical proofs:

- **GEX:** research-grade market-structure analytics and risk visibility.
- **Veritas:** probability research, calibration, and decision-support intelligence.
- **Nina:** creative revenue and release-workflow operating system.
- **Leony:** AI creative studio for media, avatar, voice, campaign, and publishing workflows.

Finance-related systems are presented only as research, simulation, risk visibility, and decision support. They are not financial advice, do not imply guaranteed returns, and do not represent autonomous capital deployment.

## Why This Matters

Agents are becoming software operators. They touch APIs, files, browsers, databases, payments, cloud services, docs, customer systems, and generated code. The hard part is no longer "can a model call a tool?"

The hard part is:

- Who authorized this action?
- Which capability was used?
- Which policy applied?
- What context was visible?
- What changed?
- What failed?
- Can a human review it?
- Can the workflow run again without becoming folklore?

Aweb is built for that layer.

## Current Collaboration Fit

Aweb is early, founder-led, and looking for serious conversations with:

- technical angels,
- AI infrastructure investors,
- startup programs,
- grant programs,
- design partners,
- teams already using AI agents in real operations.

See [COLLABORATION.md](./COLLABORATION.md) for public-safe support and partnership routes.

## Language Boundary

Use:

- Mission Control Cloud for governed AI agent work.
- Agentic orchestration platform.
- Operating system for AI production workflows.
- Control plane for agent execution.
- Human-approved sensitive actions.
- Auditable workflows and evidence.
- API Warehouse, MCP Warehouse, Maestro, Trust Runtime, OS9.

Do not use:

- AI founder with no human accountability.
- Guaranteed trading returns.
- Autonomous capital deployment.
- Crypto-first or Web3-first company.
- Alfred-era product language.
- Private investor, email, credential, legal, or wallet information.

## Contact

Daniel Wahnich  
Founder, Aweb  
business@aweb.ai  
https://aweb-wine.vercel.app/final
