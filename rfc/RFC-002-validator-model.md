# RFC-002 Validator Model

## Validator Layers

### Guardian Core Node
- Produces blocks
- Executes consensus
- Maintains full state

### Citizen Validator
- Verifies fraud proofs
- Validates state roots

### Mobile Guardian
- Light-client verification
- Header validation

### Passive Witness
- Network monitoring
- Attack reporting

## Slashing Conditions
- double signing
- invalid blocks
- censorship
- consensus attacks

## Reward Distribution
```text
40% Guardian Core
30% Citizen Validators
20% Mobile Guardians
10% Passive Witnesses
```

## Anti-Centralization
- stake caps
- geographic incentives
- hardware neutrality