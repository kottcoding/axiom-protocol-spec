# Fee Market Specification

## Fee Formula

```text
total_fee = base_fee + priority_fee
```

## Base Fee Adjustment

```text
if block_utilization > target_utilization:
  base_fee increases

if block_utilization < target_utilization:
  base_fee decreases
```

## Fee Routing

Suggested initial routing:

```text
75% validator_reward_pool
20% commons_reserve
5% minimal_burn
```

## Developer Notes

Fee calculations must use integer AXI arithmetic only. Floating point arithmetic must not be used in consensus logic.
