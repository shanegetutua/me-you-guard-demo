# Me-You-Guard (Demo) — Golden Ticket OSS Entry

**Me → You → Guard**: human intent → agent plan → **Policy Gate** (pre-execution allow/deny/require-approval) → **Audit Receipts** (Request → Decision → Outcome).

**Note:** This is a contest demo/reference implementation. It is not the full ZINYX product and does not include proprietary production internals.

## What this demo shows
A tool-using agent attempts a **high-impact action** (e.g., external file sharing). The **Policy Gate** intercepts the tool call *before execution*, applies policy, and generates an audit receipt.

## NVIDIA usage
This demo uses **NVIDIA Nemotron via NIM** for:
- short human-readable **decision explanations**
- **audit summaries** across receipts

(Policy enforcement itself is deterministic policy-as-code. The model is used for explanation and summarization only.)

## Quickstart (placeholder)
This repo currently contains the core artifacts (policy + receipt format). A runnable demo will be added next.
