# Slashing Model

## Slashable Offenses

### Critical
- double signing
- invalid finalized block
- forged consensus message

### Severe
- repeated censorship
- invalid state transition proposal
- malicious fraud proof rejection

### Moderate
- prolonged downtime
- non-participation
- invalid metadata

## Slashing Output

A slash event may include bond reduction, reward forfeiture, temporary jailing, permanent removal, or reputation penalty.

## Evidence Format

```text
SlashingEvidence {
  evidence_type
  validator_id
  block_height
  signatures
  proof_payload
  reporter
}
```
