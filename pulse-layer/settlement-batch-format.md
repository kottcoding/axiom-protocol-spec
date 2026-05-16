# Pulse Settlement Batch Format

## Batch Object

```text
PulseBatch {
  batch_id
  pulse_network_id
  previous_batch_hash
  state_commitment
  transaction_count
  fee_summary
  operator_signature
  fraud_window_end
}
```

## L1 Settlement Requirements

A batch must include valid state commitment, valid operator signature, fee payment, and previous batch reference.

## Fraud Challenge

A fraud proof may challenge invalid state transition, missing transaction, incorrect balance update, or invalid operator signature.
