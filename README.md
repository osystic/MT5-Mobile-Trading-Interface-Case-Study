# MT5 Mobile Trading Interface — Engineering Case Study

> **OSYSTIC ENGINEERING CASE STUDY · PUBLIC SHOWCASE · SANITIZED · PORTFOLIO-SAFE**

## Problem & constraints

Build a mobile MT5-style experience covering market quotes, account state, open positions, history, charts and account/settings workflows while integrating an external MT5 REST service.

## Architecture & decisions

The private delivery uses Expo / React Native with a dedicated JavaScript service layer for account connection, summary, open orders, order history and symbol data.

## Contribution & delivery

Implemented the mobile navigation/UI surfaces, account/settings flows, responsive theme utilities and provider-service integration.

## Evidence & outcomes

Private source verifies the mobile screens and REST integration. The public case study does not claim live-trading returns, production security certification or broker-provider equivalence.

## Security lesson

The historical direct-client credential flow is explicitly treated as a limitation. A hardened production design should use an approved server-side/tokenization boundary and avoid credential exposure in URLs/logging surfaces.

## Confidentiality

Account credentials, tokens, real account numbers, private broker data and delivery source are excluded.


## Public vs. private repository boundary

This repository contains **sanitized public proof only**. The confidential delivery/source repository remains private. Implementation source, account credentials, tokens, real account numbers, client identity, live account data, and protected evidence are intentionally excluded.
