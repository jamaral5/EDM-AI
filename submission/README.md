# EDM AI – Enterprise Descision Intake/Making AI

## Overview:
EDM AI's purpose is to help companiess evaluate potentially impactful decisions by making visible precedents and policy alignments, without automating approvals or rejections.

The agent supports human decision making by:
- reinterpreting/restructuring unclear decision requests
- surfacing any relevant past precedents
- confirming alignment with company policies
- explicitly notifying whether a request is consistent with past company decisions

EDM AI does not make decisions, but provides an analysis so humans can decide with context.

---

## What Problem This Solves
In large companies:
- Similar decisions can be handled inconsistently
- Context from past decisions is lost
- Teams mistakingly repeat mistakes or ignore controls
- Governance teams are forced to manually reconstruct precedent

EDM AI addresses this by acting as an offocial memory for decisions.

---

## Our Six Agents, Consolidated:

### 1. Decision Intake and Context
When a request is made, the agent extracts information such as:
- decision domain
- summary of the request
- budget or cost (if provided)
- data sensitivity
- compliance constraints
- timeline (urgency)
- stakeholders

If information is missing, the agent identifies and lists those gaps.


### 2. Decision Memory
The agent finds historically similar decisions based on:
- decision type
- data sensitivity
- context
- budget range
- approval outcomes

Results may include both approvals and rejections.


### 3. Consistency & Drift Detection
After reviewing historical precedents, the agent produces a "Consistency & Drift Signal".

This section answers one question:
"Does this request align with how similar decisions were handled in the past?"

Possible classifications:
- **Consistent** – aligns with past outcomes
- **Conditionally Consistent** – similar decisions were approved only after additional controls
- **Deviating** – would break established decision patterns
- **No Established Precedent** – a unique scenario

This signal does not recommend approve or reject.  
It makes alignment or deviation visible.


### 4. Decision Ledger 
This agent makes a record of finalized decisions. As a result, it:

- stores important details like context, reasons, and who was involved
- allows the system to look up similar past decisions for reference
- helps teams understand how and why decisions were made before
- supports transparency and audits by preserving decision history


### 5. Policy Constraint and Interpretation
The agent compares the request against company policies such as:
- data privacy and GDPR
- information security
- vendor risk management
- financial controls
- change management

The output recognizes:
- compliant areas
- insufficient information
- required approvals
- required documentation


### 6. Optional Drift Analysis
Drift analysis is only called when:
- repeated overrides are detected
- conflicting historical outcomes come up
- policy enforcement seems to be weakening over time

This prevents escalation.

---

## Synthetic Data & Demonstration:

All decisions, precedents, mergers, acquisitions, vendors, budgets, and policies used by EDM AI in this project are fake.

They were created to
- demonstrate a realistic decision history
- simulate past security approvals and cross-border mergers
- show how an official memory and precedent enforcement would work in a real company

No real companies, transactions, or data are used for the purpose of this hackathon.

---

## Example Use Cases
- Vendor on-boarding and renewals
- Cross-border data handling
- Security/compliance approvals
- Mergers and acquisitions
- High-risk operating changes


