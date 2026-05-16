# Consensus Overview

## Testnet v1 Recommendation

Axiom should start with a conservative PoS + BFT-style finality model for Testnet v1. Avoid inventing a completely new consensus mechanism before simulation, adversarial testing, formal review, and independent audit.

## Consensus Flow

```text
1. Validator selection
2. Block proposal
3. Block validation
4. Pre-vote
5. Pre-commit
6. Finality
7. Reward / penalty accounting
```

## Safety Assumption

The network remains safe if less than the Byzantine threshold of effective voting power behaves maliciously.

## Liveness Assumption

The network remains live if enough honest validators are online and able to communicate.
