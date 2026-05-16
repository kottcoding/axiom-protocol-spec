# Validator Reward Simulator Specification

## Objective

Model validator reward distribution before testnet.

## Inputs

- validator count
- stake per validator
- uptime score
- slashing score
- fee revenue
- annual emission
- reward pool percentage

## Reward Score

```text
reward_score = stake_weight + uptime_score + correctness_score + decentralization_bonus - penalty_score
```

## Output

- reward per validator
- validator APR estimate
- concentration risk
- post-year-100 sustainability
