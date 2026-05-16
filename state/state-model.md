# Axiom State Model

## Global State

```text
GlobalState {
  chain_id
  block_height
  epoch_id
  total_supply_axi
  circulating_supply_axi
  burned_supply_axi
  accounts_root
  validators_root
  system_contracts_root
}
```

## Account State

```text
Account {
  address
  balance_axi
  nonce
  account_type
  permissions
}
```

## Account Types

```text
STANDARD
SMART_ACCOUNT
VALIDATOR_ACCOUNT
FOUNDER_VESTING_ACCOUNT
AI_AGENT_ACCOUNT
SYSTEM_ACCOUNT
```

## Validator State

```text
Validator {
  validator_id
  operator_address
  stake_axi
  status
  uptime_score
  slashing_score
  reward_score
  last_active_epoch
}
```

## State Transition Rule

Every valid block transforms State(N) into State(N+1). The transition must be deterministic across all honest nodes.
