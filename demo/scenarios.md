# PrecedentAI – Demo Scenarios

This document outlines two demonstration scenarios used to showcase how PrecedentAI captures institutional knowledge, enforces decision consistency, and prevents costly repeat mistakes.

---

## Scenario 1: Preventing a Repeat Compliance Mistake

### Context
A product team wants to quickly approve a new vendor to handle logs for EU customers. It is costly and touches customer data, but they’re under time pressure.

### Decision Dialog:
“We need to approve Vendor Beta fast.
It’ll cost $500k a year.
They’ll handle EU customer data.
We need this for an upcoming launch.”

### What EDM AI Does:
- Pulls out the important details (vendor name, cost, EU data, sensitive info)
- Checks past decisions
- Checks company policies and compliance rules
- Looks for patterns where teams have recently bent the rules

### What it Finds:
- This exact vendor was rejected before for EU data issues
- The request breaks multiple compliance rules (EU data residency, SOC 2)
- Teams have recently been overriding similar rules more often (a red flag)

### Recommendation:
**Decision:** Do Not Approve (Pending Remediation)  

Why:
- This goes against a past decision
- It breaks established compliance rules

What to Do Instead:
- Require proof that EU data stays in the EU
- Require a security audit before reconsidering

### Outcome:
The company avoids repeating a compliance failure and gives the team a clear checklist to move forward safely.

---

## Scenario 2: Capturing Institutional Knowledge for Future Decisions

### Context
The Security and Legal teams approve a new policy intended to standardize vendor security requirements across the organization.

### Input (Decision Intake)
"Effective immediately, all third-party vendors that handle customer PII must maintain SOC 2 Type II certification prior to production use."

### System Actions
- The Decision Intake Agent identifies the request as a policy-level decision.
- The Rationale Extractor captures the intent, scope, and enforcement conditions.
- The Decision Ledger Agent records the policy decision as institutional precedent.

### Output (Decision Recorded)
**Decision:** Approved  
**Scope:** All procurement and security reviews involving customer data  
**Rationale:** Standardizes security expectations, reduces vendor risk, and aligns with regulatory obligations.  
**Enforcement:** This policy will be automatically evaluated during future vendor approval requests.

### Outcome
The organization’s institutional memory is updated, ensuring consistent enforcement of the policy in future decisions without relying on individual recollection.

---

## Summary
These scenarios demonstrate how PrecedentAI:
- Prevents repeat mistakes by referencing past decisions
- Enforces compliance through policy-aware recommendations
- Learns over time by capturing and applying institutional knowledge

