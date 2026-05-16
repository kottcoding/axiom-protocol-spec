# Developer Implementation Roadmap

## Phase A: Simulator Layer

Build first:
- token_units
- emission_schedule
- fee_market
- founder_vesting
- validator_rewards

Goal: prove the economics before building the chain.

## Phase B: Protocol Data Model

Build deterministic structures:
- Transaction object
- Block object
- Account state
- Validator state
- Epoch state

## Phase C: State Transition Engine

Build:
- transaction validation
- balance update
- fee charging
- reward distribution
- block execution

## Phase D: Minimal Node

Build:
- mempool
- block proposal
- block validation
- local persistence
- simple P2P mock

## Phase E: Testnet v1

Build:
- multi-node network
- validator registry
- faucet
- explorer
- wallet
- basic monitoring
