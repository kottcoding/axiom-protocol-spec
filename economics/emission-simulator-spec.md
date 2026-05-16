# Emission Simulator Specification

## Objective

Simulate AXM issuance over 100 years.

## Constants

```text
MAX_SUPPLY_AXM = 100,000,000
ANNUAL_EMISSION_AXM = 1,000,000
EMISSION_YEARS = 100
AXI_PER_AXM = 100,000,000
```

## Required Outputs

The simulator should output year, annual emission, cumulative supply, remaining supply, and emission percentage complete.

## Formula

```text
cumulative_supply(year) = min(year * 1,000,000 AXM, 100,000,000 AXM)
```

## Post-Emission

For year greater than 100, annual_emission is 0.
