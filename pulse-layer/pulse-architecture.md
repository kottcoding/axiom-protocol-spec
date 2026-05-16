# Pulse Micropayment Architecture

## Purpose

Pulse is the Layer-2 micropayment layer for Axiom.

## Use Cases

- AI API payments
- streaming payments
- merchant QR payments
- content payments
- game transactions
- machine-to-machine settlement

## Flow

```text
User/AI locks funds on L1
        ↓
Pulse executes many small payments
        ↓
Pulse batches state
        ↓
Batch settles to Axiom L1
```

## Security Model

Pulse security depends on cryptographic commitments, challenge windows, L1 settlement finality, and fraud proofs.
