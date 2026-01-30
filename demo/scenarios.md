# PrecedentAI – Demo Scenarios

This document outlines two demonstration scenarios used to showcase how PrecedentAI captures institutional knowledge, enforces decision consistency, and prevents costly repeat mistakes.

---

## Scenario 1: Preventing a Repeat Compliance Mistake

### Context
A product team is requesting approval to onboard a new log management vendor to support EU customer environments. The request is time-sensitive due to operational pressure.

### Input (Decision Intake)
"We need to approve Vendor Beta for centralized log aggregation for EU customers.  
Estimated annual cost is $500,000.  
This vendor will process customer telemetry and logs.  
We need to move quickly to support upcoming launches."

### System Actions
- The Decision Intake Agent extracts key attributes (vendor, budget, data region, data classification).
- The Decision Memory Agent identifies a prior decision involving the same vendor.
- The Policy Interpreter Agent evaluates applicable compliance requirements.
- The Consistency & Drift Detection Agent assesses alignment with past decisions and recent governance trends.

### Key Findings
- A previous decision (DEC-002) rejected Vendor Beta due to EU data residency and subprocessor concerns.
- Current request triggers multiple high-severity policies, including EU data residency and SOC 2 requirements.
- Drift analysis indicates an increase in recent overrides related to similar vendors.

### Output (Recommendation)
**Decision:** Do Not Approve (Pending Remediation)  
**Rationale:** The request conflicts with prior precedent and violates established compliance policies.  
**Recommendation:** Require documented EU-only data residency guarantees and completion of a third-party security audit before reconsideration.

### Outcome
A potential repeat compliance failure is avoided, and the team is provided with a clear, actionable path forward.

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

