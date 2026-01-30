# PrecedentAI
**Institutional Memory and Decision Governance for Enterprises**

---

## Problem Statement

Enterprises make thousands of decisions every year across procurement, security, legal, and engineering teams.  
However, the rationale behind these decisions is often lost over time—buried in emails, chat threads, tickets, or held only in people’s memories.

As a result:
- Teams repeatedly re-litigate the same decisions
- Past rejections are forgotten and mistakes are repeated
- Policies are inconsistently enforced
- Risk tolerance gradually shifts without visibility or intent

This loss of institutional memory leads to **increased compliance risk, inconsistent governance, and costly errors**.

---

## Solution Overview

**PrecedentAI** is a multi-agent system built with **IBM watsonx Orchestrate** that captures how decisions are made and enforces consistency over time.

Rather than acting as a simple search or chatbot tool, PrecedentAI models the **decision lifecycle**:
- Intake of new decision requests
- Retrieval of relevant historical precedents
- Policy interpretation and enforcement
- Detection of inconsistencies and governance drift
- Recommendation with explainable tradeoffs
- Recording of final decisions as auditable institutional memory

Each decision strengthens the system, reducing reliance on tribal knowledge and manual oversight.

---

## Key Capabilities

### 1. Decision Memory
PrecedentAI maintains a structured record of past decisions, including:
- What was decided
- Why it was decided
- Constraints and risks considered
- Who approved it

This allows new decisions to be evaluated in the context of organizational precedent.

### 2. Policy-Aware Enforcement
Enterprise policies (e.g., SOC 2 requirements, data residency, budget thresholds) are interpreted and applied consistently during decision evaluation.

Violations and missing requirements are explicitly identified rather than implicitly assumed.

### 3. Consistency and Drift Detection
PrecedentAI compares new requests against past decisions to:
- Flag contradictions
- Highlight repeat exceptions
- Surface trends indicating policy drift over time

This enables proactive governance rather than reactive review.

### 4. Explainable Recommendations
Instead of binary approvals or rejections, the system produces structured recommendations that include:
- Referenced precedents
- Policy impacts
- Risk tradeoffs
- Clear next steps

### 5. Institutional Learning
Final decisions—including overrides and exceptions—are recorded in a decision ledger, ensuring that future decisions benefit from prior context and justification.

---

## Architecture and Agent Design

PrecedentAI is implemented as a **multi-agent system** using watsonx Orchestrate, with each agent responsible for a distinct role:

- **Decision Intake Agent**  
  Parses incoming requests and extracts structured decision attributes.

- **Decision Memory Agent**  
  Retrieves and ranks relevant past decisions based on similarity.

- **Policy & Constraint Interpreter Agent**  
  Evaluates applicable enterprise policies and identifies violations or missing information.

- **Consistency & Drift Detection Agent**  
  Compares current decisions to precedent and analyzes governance trends over time.

- **Recommendation & Tradeoff Agent**  
  Synthesizes findings into an explainable recommendation.

- **Decision Ledger Agent**  
  Records the final decision and rationale as institutional memory.

Agents collaborate through watsonx Orchestrate, demonstrating end-to-end orchestration rather than isolated automation.

---

## Demo Scenarios

The demo includes two scenarios:

1. **Preventing a Repeat Compliance Mistake**  
   A time-sensitive vendor approval request is evaluated against past rejections and current policies, preventing a costly repeat error.

2. **Capturing Institutional Knowledge**  
   A new security policy is approved and recorded, ensuring consistent enforcement across future decisions.

Full demo scripts are available in `demo/scenarios.md`.

---

## Why watsonx Orchestrate

watsonx Orchestrate enables PrecedentAI to:
- Model complex, real-world decision workflows
- Coordinate multiple specialized agents
- Integrate knowledge, tools, and human-in-the-loop approvals
- Provide explainability and governance required for enterprise AI adoption

This solution aligns directly with enterprise needs for **trusted, auditable, and scalable AI systems**.

---

## Impact

PrecedentAI helps organizations:
- Reduce repeat mistakes
- Enforce policies consistently
- Improve auditability and compliance
- Preserve institutional knowledge despite employee turnover
- Make faster, better-informed decisions at scale

---

## Team

Built as part of the IBM AI Demystified Hackathon using watsonx Orchestrate.

