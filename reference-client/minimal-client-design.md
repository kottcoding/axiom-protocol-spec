# Minimal Reference Client Design

## Components

```text
axiom-node/
  core/
  state/
  txpool/
  consensus/
  networking/
  rpc/
  storage/
```

## Minimum Features

- create account
- send transaction
- validate transaction
- build block
- validate block
- apply state transition
- persist state
- expose RPC

## Recommended Language

For early prototype: Go, Rust, or TypeScript. Recommendation: start simulator in TypeScript or Python, then build node prototype in Go or Rust.
