# Me-You-Guard (Demo) — Golden Ticket OSS Entry

A **pre-execution policy gate** for tool-using agents: **allow / deny / require approval** before high-impact actions run, and emit an **audit trail** per action (Request → Decision → Outcome).

**NVIDIA:** Uses **Nemotron via NIM** for human-readable explanations and summaries (non-authoritative).

**Note:** Contest demo/reference only. Production internals intentionally omitted.

## What this demo shows
A tool-using agent attempts a **high-impact action** (e.g., external file sharing). The **Policy Gate** intercepts the tool call *before execution*, evaluates the action against org-defined rules, and emits an audit trail entry.

The model is used only to produce human-readable rationale and summaries; it does not make the enforcement decision.

## Quickstart (Status)
A runnable demo may be added later.

