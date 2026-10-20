# MT5 Mobile Trading Interface

## P — Problem & constraints

Create a mobile interface for core MT5 account and market workflows while working through an external REST integration boundary. The delivered application needed to organize quotes, open positions, charts, history, account connection and settings into a mobile-first experience without representing the client application itself as a hardened credential vault or as proof of live-trading performance.

## A — Architecture & decisions

The private delivery uses an Expo / React Native application with a dedicated JavaScript service layer between the mobile UI and an external MT5 REST provider. The service layer covers account connection, account summary, open orders or positions, order history, symbol discovery and symbol-parameter retrieval. The UI is separated into quotes, trade, chart, history, account and settings surfaces.

A key security decision in this case study is to document the historical direct-client credential flow as a limitation rather than hide it. A production-hardening path would place credential exchange or tokenization behind an approved server-side boundary and minimize the chance of passwords or tokens appearing in URLs, logs, analytics or screenshots.

## C — Contribution & delivery

OSYSTIC delivered the mobile navigation and screen structure, account/settings workflows, responsive theme utilities and the provider-facing MT5 service abstraction. The retained private source demonstrates how mobile presentation, account state and remote trading-platform data were integrated without publishing real account credentials or protected broker information in this public repository.

## Engineering highlights

- Structured the application around dedicated quotes, trade, chart, history and settings/account screens rather than one monolithic interface.
- Isolated MT5 REST calls inside a service abstraction for account, order-history and symbol-related requests.
- Preserved a clear security boundary in the public case study by explicitly documenting the direct-client credential-flow limitation.
- Kept public evidence separate from real account numbers, credentials, session tokens and live account data.

## Technology stack

- Expo
- React Native
- JavaScript
- REST API integration
- MetaTrader 5 / MT5 service integration

## E — Evidence & outcomes

The private repository contains the Expo application source, screen modules, account/settings components and the MT5 REST service abstraction. That evidence supports the engineering claims made here about implemented mobile workflows and integration capability.

The evidence does **not** establish profitable trading, broker equivalence, production security certification, guaranteed execution quality or future financial performance. The public outcome is therefore limited to a verified mobile-interface and integration delivery with its security limitations disclosed.

## Confidentiality

Public proof excludes delivery source, client identity, broker/account credentials, session tokens, real account numbers, live account data and private provider details. The confidential implementation remains in the private delivery repository.
