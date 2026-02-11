\# ClawShield



\*\*Governance sidecar for OpenExec\*\*



ClawShield exists to make autonomous execution \*\*legible\*\*.



It does not run tasks.  

It does not modify behavior.  

It does not fix mistakes.



ClawShield defines \*\*policy boundaries\*\*, evaluates actions \*\*before execution\*\*, and produces \*\*verifiable receipts\*\* of what was allowed or denied.



When systems act, ClawShield makes those actions \*\*explainable\*\*.



This matters when actions must be reviewed, shared, or defended outside the system that performed them.



---

## System architecture

This project is part of a three-layer governed execution system:

- **OpenExec** executes actions deterministically.
- **ClawShield** governs whether actions are permitted before execution.
- **ClawLedger** records immutable receipts of what was decided and why.

Execution, governance, and evidence are intentionally separated.
No layer replaces another.
Together, they make autonomous systems legible, reviewable, and defensible.




\## What you are looking at



If you continue, you will enter a \*\*governance workspace\*\* containing:



\- \*\*Policies\*\* that define what an agent \*may\* attempt  

\- \*\*Preflight checks\*\* that evaluate actions before execution  

\- \*\*Receipts\*\* that record governance decisions immutably  



Nothing runs automatically.  

No background enforcement is active by default.



ClawShield governs decisions.  

Other systems execute them.



---



\## What ClawShield is not



ClawShield is \*\*not\*\*:



\- An execution engine  

\- An automation framework  

\- An AI agent  

\- A monitoring or surveillance system  



It does not schedule work.  

It does not retry failures.  

It does not intervene after execution begins.



ClawShield draws boundaries.  

It does not cross them.



---



\## Governance model



ClawShield operates in \*\*default-deny\*\* mode.



Every action is evaluated explicitly against policy.  

If a policy does not allow it, the action is denied.



A denial is not an error.  

It is a boundary being enforced.



Each decision produces a \*\*sealed receipt\*\* containing:

\- The evaluated action

\- The target

\- The policy hash

\- The decision (allowed or denied)

\- A timestamp

\- A sealed marker indicating immutability



Receipts are evidence.  

They do not expire.



---



\## Relationship to OpenExec



OpenExec executes tasks.



ClawShield governs whether those tasks \*should be executed\*.



ClawShield does not fork OpenExec.  

It does not wrap execution.  

It does not intercept runtime behavior.



It evaluates intent \*\*before execution\*\* and records the decision.



---



\## Modes



\### Free — Learning Governance

\- Manual preflight checks  

\- View receipts  

\- Learn policy boundaries  

\- Up to 5 active policies  



\### Governed — Operating with Responsibility

\- Export evidence  

\- Continuous enforcement  

\- Programmatic access  

\- Unlimited policies  

\- Policy templates  



Governed mode does not make decisions safer.  

It makes decisions \*\*survivable\*\*.



---



\## Design principles



\- Governance must be \*\*explicit\*\*

\- Boundaries must be \*\*visible\*\*

\- Decisions must be \*\*provable\*\*

\- Evidence must be \*\*portable\*\*

\- Silence is preferable to hype



If ClawShield blocks something you did not expect, that is a signal — not a failure.



---



\## Status



This repository is the \*\*canonical reference\*\* for ClawShield’s governance model.



The running application and UI are implemented elsewhere.  

This repository defines intent, scope, and guarantees.



---



\## License



To be defined.

---

## Related repositories

- **OpenExec** — Deterministic execution engine  
  https://github.com/trendinghot/OpenExec

- **ClawLedger** — Witness ledger for governed execution  
  https://github.com/trendinghot/clawledger







