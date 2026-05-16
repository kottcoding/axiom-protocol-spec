# Validator Lifecycle

## States

```text
CANDIDATE
ACTIVE
JAILED
EXITING
INACTIVE
SLASHED
```

## Registration

A validator must submit operator address, consensus public key, bond amount, metadata, and endpoint information.

## Activation

Activation requires minimum bond, valid key, network acceptance, and epoch boundary.

## Jailing

A validator may be jailed for downtime, double signing, invalid block, or censorship evidence.

## Exit

Validator exit requires an exit request, unbonding period, and no pending slashing evidence.
