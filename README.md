# Me-You-Guard (demo)

A **pre-execution policy gate** for tool-using agents: **ALLOW / DENY / REQUIRE APPROVAL** before high-impact actions run, and emit an **audit receipt** per attempt (**Request → Decision → Outcome**).

> **IP / disclosure posture (strict):** This repository intentionally describes **outcomes and externally observable behavior only**. **Implementation details, system placement/architecture, policy mechanics, schemas, and enforcement internals are intentionally omitted** to avoid disclosure.

---

## What it is

**Me-You-Guard (demo)** demonstrates a simple idea:

- Models and agents can propose actions.
- **Execution must be governed** before irreversible actions occur.
- Every attempt should be **accountable** via an action-level record.

**We don’t replace models or agents — we govern execution and keep action-level records for accountability.**

---

## What the demo shows

For an attempted high-impact action, the demo produces:

1) A **Request** (the action attempt, described at a high level)  
2) A **Decision**: **ALLOW / DENY / REQUIRE APPROVAL**  
3) An **Outcome** (executed / blocked / pending)  
4) An **audit receipt** that captures **Request → Decision → Outcome** per attempt

> No policy formats, rule examples, configuration mechanics, receipt field lists, storage details, or enforcement methods are published in this repo.

---

## Why this exists

As AI systems move from “answers” to **actions**, mistakes become **operational incidents** when an agent can trigger irreversible changes (send, change, export, deploy).

This demo focuses on the last-mile safety pattern:

- **Stop bad actions before execution**
- **Require approval** for risky actions
- Keep **accountability per attempt**

---

## NVIDIA usage

This demo uses **NVIDIA Nemotron via NIM** to generate **human-readable explanations** of decisions (**non-authoritative**, for clarity only).

---

## How to evaluate

This repository is intended to be evaluated by **observable behavior**, not internals:

- Confirm the demo shows **ALLOW / DENY / REQUIRE APPROVAL**
- Confirm each attempt produces an audit receipt at the label level: **Request → Decision → Outcome**
- Confirm Nemotron/NIM output is presented as explanatory text (**non-authoritative**)

---

## Contest note

This repository is an **open-source contest demo/reference** intended for NVIDIA GTC Golden Ticket entry.

Hashtags: **#NVIDIAGTC #GOLDENTICKET**

---

## Security & disclosure constraints

Public materials in this repo **do not include**:
- architecture or placement details
- implementation procedures or integration instructions
- policy logic, rule examples, or configuration mechanics
- receipt schemas/field listings or structured examples that enable replication
- connector specifics to third-party platforms

If deeper details are needed, those are **NDA-scoped**.

---

## License

Add a permissive open-source license (e.g., **Apache-2.0** or **MIT**) before wider distribution.

---

## Contributing

Contributions are welcome, but must respect the repo’s **non-disclosure posture**:
- Keep additions at **outcomes/behavior level**
- Avoid adding implementation details, schemas, policy mechanics, or integration instructions

---

## Disclaimer

This is a **demo/reference** project. It is not presented as a production system, and it does not provide operational guarantees.
Commit message (use this)
