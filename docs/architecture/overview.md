# Public Architecture Overview

## Design stance

Novera is designed as an **EVM-first, chain-agnostic** modular platform. The product and domain model should not depend on a single distributed ledger.

## Logical layers

| Layer | Public purpose | Current status |
|---|---|---|
| Experience | Operator and stakeholder lifecycle dashboards | Planned |
| Application | API, workflow orchestration, authorization, and audit services | Private MVP foundation |
| Domain | NovaID, NovaRegistry, NovaDeed, policy, and lifecycle models | Private MVP foundation |
| Data | Relational records, append-only events, and future document references | Private MVP foundation |
| Integration | Identity, compliance, legal, payment, ledger, and oracle adapters | Mock-only boundaries |
| Settlement | Future EVM and optional enterprise-ledger adapters | Deferred |

## Chain strategy

The future deployment environment will be selected against settlement assurance, operational risk, cost, ecosystem maturity, Chainlink support, institutional compatibility, upgrade governance, and interoperability requirements.

- **Candidate EVM environments:** Base, Arbitrum, Ethereum mainnet, and other suitable environments.
- **Hedera:** optional future adapter where enterprise or customer requirements justify it.
- **Chainlink CRE:** possible future tool for verifiable off-chain workflows and external data handling.
- **CCIP:** considered only where cross-chain functionality is demonstrably required.

No selection, contract deployment, testnet connection, or live ledger activity is represented by this repository.

## Trust boundaries

Future integrations must be isolated behind explicit adapters, policy controls, event records, and auditable authorization. The platform must never treat a blockchain record by itself as proof of identity, legal title, asset quality, reserve backing, regulatory eligibility, or payment finality.
