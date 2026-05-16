# State Transition Function

## Function

```text
apply_block(previous_state, block) -> new_state
```

## Required Steps

1. Verify block header
2. Verify proposer identity
3. Verify validator signatures
4. Verify transaction root
5. Execute transactions in canonical order
6. Charge fees
7. Apply rewards
8. Update supply accounting
9. Recalculate state root
10. Return new state

## Transaction Execution

```text
apply_transaction(state, tx):
  assert tx.signature_valid
  assert tx.nonce == account.nonce + 1
  assert account.balance >= tx.amount + tx.fee
  debit sender
  credit receiver
  route fee
  increment nonce
```

## Invalid Transactions

A transaction is invalid if signature is invalid, nonce is incorrect, balance is insufficient, fee is below minimum, account permission rejects action, or AI policy rejects action.
