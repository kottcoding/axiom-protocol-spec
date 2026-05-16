# AI Agent Account Specification

## Account Goal

Allow AI agents to transact without giving them unrestricted control over user funds.

## Required Fields

```text
AIAgentAccount {
  owner_address
  agent_id
  session_public_key
  daily_limit_axi
  per_tx_limit_axi
  allowed_contracts
  expiration
  revoke_nonce
}
```

## Required Controls

- session key
- spending limit
- contract whitelist
- expiration
- emergency revoke
- human approval threshold
- audit log

## Transaction Validation

AI transaction is valid only if session key is valid, session has not expired, amount is within per transaction limit, daily usage is within daily limit, target contract is allowed, and owner has not revoked permission.
