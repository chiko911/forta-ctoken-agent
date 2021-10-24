# Compound Agent

## Description

This agent monitors the Compound protocol and alerts when:

- cToken (cEther) exchange rate goes down

## Supported Chains

- Ethereum

## Alerts

- COMPOUND-4

  - Fired when a COMP distribution occurs that is at least twice as much as accrued
  - Severity is always set to "High"
  - Type is always set to "Suspicious"
  - Metadata fields included:
    - `receiver` - the address that received the COMP tokens
    - `compDistributed` - the amount of COMP distributed to receiver
    - `compAccrued` - the amount of COMP accrued by receiver in the previous block

## Test Data

The agent behaviour can be verified with the following transactions:
