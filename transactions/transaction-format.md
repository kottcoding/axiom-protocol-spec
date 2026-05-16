# Transaction Format

## Base Transaction

```text
Transaction {
  version
  chain_id
  sender
  receiver
  amount_axi
  nonce
  gas_limit
  max_base_fee_axi
  priority_fee_axi
  payload
  signature
}
```

## Transaction Types

```text
TRANSFER
SMART_CONTRACT_CALL
VALIDATOR_REGISTER
VALIDATOR_UNBOND
AI_AGENT_ACTION
PULSE_SETTLEMENT
FOUNDER_VESTING_CLAIM
SYSTEM
```

## Validation Requirements

A transaction must pass signature verification, replay protection, fee sufficiency, balance sufficiency, permission check, and protocol rule check.

## Internal Accounting

All transaction amounts must be represented in AXI.

```text
1 AXM = 100,000,000 AXI
```
