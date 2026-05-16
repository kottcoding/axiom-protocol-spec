# AI Risk Engine

## Purpose

Detect and prevent dangerous AI-driven financial actions.

## Risk Signals

- unusual transaction frequency
- new contract target
- large amount
- repeated failed calls
- abnormal routing
- cross-agent coordination

## Risk Response

```text
LOW: allow
MEDIUM: require confirmation
HIGH: pause agent
CRITICAL: emergency revoke
```

## Developer Requirement

Risk engine decisions must be explainable to the owner.
