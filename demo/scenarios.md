# PrecedentAI – Demo Scenarios

This document outlines two demonstration scenarios used to showcase how PrecedentAI captures institutional knowledge, enforces decision consistency, and prevents costly repeat mistakes.

---

## Scenario 1: Preventing a Compliance Mistake from Happening Again

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
**Decision:** 
Do Not Approve.

**Why:**
- This goes against a past decision
- It breaks established compliance rules

**What to Do Instead:**
- Require proof that EU data stays in the EU
- Require a security audit before reconsidering

### Outcome:
The company avoids repeating a compliance failure and gives the team a clear checklist to move forward safely.

---

## Scenario 2: Remembering a New Rule So People Do Not Forget Later

### Context
Security and Legal teams approve a new rule regarding how vendors handle customer data.

### Decision Dialog:
“Any vendor that handles customer PII must have SOC 2 Type II certification before going live.”

### What EDM AI Does:
- Recognizes this is a policy decision, not just a one-off approval
- Records the rule, why it exists, and where it applies
- Saves it as official company knowledge

### What it Finds:
**Decision:** 
Approved  

**From now on:**
- Every vendor request involving customer data is automatically checked against this rule
- No one has to “remember” it
- The rule is enforced consistently, even when teams change

### Outcome:
The organization’s institutional memory is updated, making sure the policy is enforced in future decisions.

---

## Summary:
EDM AI is a company’s long-term memory and rule enforcer. It makes sure decisions are compliant, consistent, and concise.

