# PrecedentAI – Decision Intake & Consistency Agent

## Overview
PrecedentAI is an enterprise decision-intake and governance agent built using watsonx Orchestrate.  
Its purpose is to help organizations evaluate **high-impact decisions** by making **institutional precedent and policy alignment visible**, without automating approvals or rejections.

The agent supports **human-in-the-loop decision making** by:
- structuring unclear decision requests
- surfacing relevant historical precedents
- checking alignment with enterprise policies
- explicitly signaling whether a request is consistent with past decisions

PrecedentAI does **not** make decisions. It provides structured analysis so humans can decide with context.

---

## What Problem This Solves
In large organizations:
- Similar decisions are often handled inconsistently over time
- Context from past decisions is lost
- Teams repeat mistakes or bypass controls unintentionally
- Governance teams are forced to manually reconstruct precedent

PrecedentAI addresses this by acting as **institutional memory** for decisions.

---

## Agent Responsibilities

### 1. Decision Intake & Context Extraction
When a request is submitted, the agent extracts key information such as:
- decision domain
- summary of the request
- budget or cost (if provided)
- data sensitivity
- compliance constraints
- timeline or urgency
- stakeholders or requesting teams

If information is missing or unclear, the agent explicitly lists those gaps.

---

### 2. Precedent Search
The agent invokes a Precedent Search Tool to find historically similar decisions based on:
- decision type
- data sensitivity
- regulatory context
- budget range
- approval outcomes

Results may include both approvals and rejections.

---

### 3. Consistency & Drift Signal (Always Emitted)
After reviewing historical precedents, the agent produces a **Consistency & Drift Signal**.

This section answers one question:
> *Does this request align with how similar decisions were handled in the past?*

Possible classifications:
- **Consistent** – aligns with historical outcomes
- **Conditionally Consistent** – similar decisions were approved only after additional controls
- **Deviating** – would break established decision patterns
- **No Established Precedent** – represents a novel scenario

This signal **does not recommend approve or reject**.  
It simply makes alignment or deviation visible.

---

### 4. Policy Check
The agent evaluates the request against enterprise policies, such as:
- data privacy and GDPR
- information security
- vendor risk management
- financial controls
- change management

The output highlights:
- compliant areas
- insufficient information
- required approvals or documentation

---

### 5. Optional Drift Analysis (Escalation Only)
Trend-level drift analysis is only invoked when:
- repeated overrides are detected
- conflicting historical outcomes emerge
- policy enforcement appears to be weakening over time

This prevents unnecessary noise and escalation.

---

## Synthetic Data & Demonstration Context

All historical decisions, precedents, mergers, acquisitions, vendors, budgets, and policies used by PrecedentAI in this project are **synthetic and fictional**.

They were intentionally created to:
- simulate realistic enterprise decision histories
- model past vendor onboarding, security approvals, and cross-border mergers
- demonstrate how institutional memory and precedent enforcement would function in a real organization

No real companies, transactions, or proprietary data are referenced.

The structure, tone, and governance logic reflect **real-world enterprise practices**, but the data itself is **fabricated solely for demonstration and evaluation purposes**.

This approach allows the system to demonstrate:
- decision consistency analysis
- governance pattern recognition
- drift detection behavior
- human-in-the-loop decision support

without exposing sensitive or confidential information.

---

## Design Principles
- **Human-in-the-loop**: The agent never makes final decisions
- **Explainability first**: All conclusions are traceable to precedent or policy
- **Restraint**: Advanced analysis is only triggered when justified
- **Enterprise realism**: Mirrors real governance workflows

---

## Example Use Cases
- Vendor onboarding and renewals
- Cross-border data handling decisions
- Security and compliance approvals
- Mergers & acquisitions intake
- High-risk operational changes

---

## Why This Matters
PrecedentAI helps organizations:
- enforce decision consistency
- reduce governance risk
- preserve institutional knowledge
- improve auditability
- avoid repeating past mistakes

It transforms decision history into an active governance asset.

---

## Disclaimer
PrecedentAI does not approve, reject, or replace human judgment.  
All outputs are advisory and intended to support responsible enterprise decision making.
