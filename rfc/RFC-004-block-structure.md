# RFC-004 Block Structure

## Block Header
```text
- chain_id
- block_height
- previous_hash
- timestamp
- state_root
- transaction_root
```

## Block Body
- transactions
- settlement batches
- validator signatures

## Validation Lifecycle
1. Verify transactions
2. Execute state transitions
3. Calculate roots
4. Validate signatures
5. Finalize block

## Fraud Proofs
Enable lightweight verification for decentralized security.