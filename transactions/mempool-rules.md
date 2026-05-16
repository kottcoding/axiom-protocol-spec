# Mempool Rules

## Admission Rules

A transaction may enter the mempool only if it has a valid signature, correct chain_id, fee above current minimum, valid or near-future nonce, and payload size within limits.

## Ordering Rules

Initial ordering:

```text
priority_score = priority_fee_axi + age_score - spam_penalty
```

## Spam Protection

- dynamic minimum fee
- per-account pending transaction limit
- AI-agent rate limits
- payload size caps
- duplicate rejection

## AI Transaction Handling

AI transactions must include agent_id, owner_address, policy_id, session_key, and expiration.
