# Compound Agent

## Description

This agent monitors the Compound protocol and alerts when:

- cToken (cEther) exchange rate goes down

## Supported Chains

- Ethereum

## Alerts

- COMPOUND-4

  - Fired when a Token (cEther) exchange rate goes down
  - Severity is always set to "High"
  - Type is always set to "Suspicious"
  - Metadata fields included:
    - `ctokenCurrentExchangeRate`
    - `ctokenPreviousExchangeRate`

## Test Data

The agent behaviour can be verified with the following transactions:
