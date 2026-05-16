# RFC-003 Transaction & Fee Model

## Transaction Structure
- sender
- receiver
- amount
- nonce
- gas_limit
- signature

## Dynamic Fee Market
```text
TotalFee = BaseFee + PriorityFee
```

## Base Fee
Adjusted according to:
- block congestion
- mempool demand
- network utilization

## Fee Allocation
- Validator pool
- Commons reserve
- Burn mechanism

## AI Economy Support
- streaming payments
- autonomous recurring settlement
- AI micropayments