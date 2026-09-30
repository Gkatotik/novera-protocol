![Novera Protocol](assets/novera-protocol-logo.png)

# Novera Protocol

> **Your Assets, Your Control, Your Future.**
>
> Infrastructure for real-world assets.

This repository is Novera Protocol's public product, architecture, roadmap, governance, and disclosure record. It is not the private implementation repository or a production platform.

## Start here

| Resource | Purpose |
|---|---|
| [Website](https://noveraprotocol.org/) | Product narrative and institutional overview |
| [Product status](https://noveraprotocol.org/status) | Canonical scope, maturity, limitations, and evidence |
| [Architecture](https://noveraprotocol.org/architecture) | Interactive system model and current network posture |
| [Developer documentation](https://noveraprotocol.org/docs) | Concepts, illustrative schemas, proposed interfaces, and MVP evaluation |
| [Public roadmap](docs/product/roadmap.md) | Version-controlled Now / Next / Later sequence |
| [Public disclosures](docs/governance/public-disclosures.md) | NOVA, NovaStable, governance, and no-offer boundaries |

## Current status

Novera is at a **foundation and synthetic lifecycle MVP stage**.

The public MVP is designed to represent participant state, asset records, ownership-document workflow state, policy decisions, provenance, and lifecycle events using synthetic data. It does not provide real identity verification, legal title transfer, payment processing, custody, production settlement, asset tokenization, or a live blockchain network.

## Canonical product state

| Component | State | Current scope |
|---|---|---|
| NovaID | MVP mock | Synthetic participant and verification-state model; no real KYC/KYB or identity documents |
| NovaRegistry | MVP | Synthetic asset records, relationships, versions, provenance, and lifecycle events |
| NovaDeed | MVP mock | Synthetic document-package, evidence, review, and approval states; no deed or legal title transfer |
| NovaScan | Planned | Future read-only lifecycle and evidence view; no live explorer |
| Compliance Engine | Conditional | Future policy and provider-integration boundary; no current compliance determination |
| Legal API Gateway | Conditional | Future legal-provider integration boundary; no current legal service |
| Settlement adapter | Under evaluation | Replaceable EVM-first, chain-agnostic interface; no production chain selected |
| NovaPay | Not in MVP | No payment, custody, escrow, reconciliation, or settlement processing |
| NOVA / NovaStable | Not in MVP | No token or stable-value asset issued, offered, reserved, or deployed |

Read the [public status model](docs/product/status-model.md) for the vocabulary used across the website and repository.

## Architecture position

- **EVM-first and chain-agnostic:** domain and workflow layers are designed to avoid coupling to one blockchain.
- **No production chain is selected:** Base is a leading candidate under evaluation only.
- **Hedera is optional:** it may be assessed as a future adapter where a validated use case justifies it.
- **Chainlink is conditional:** CRE, CCIP, and Proof of Reserve are potential future integrations, not active dependencies or partnerships.
- **External authorities remain external:** identity providers, legal professionals, registries, payment providers, and other institutions remain responsible for their authoritative functions.

Read the [architecture overview](docs/architecture/overview.md) and the website's [technology and regulatory boundaries](https://noveraprotocol.org/boundaries).

## Repository boundaries

### Published here

- Public product and architecture summaries
- High-level roadmap and governance position
- Public security-reporting and contribution guidance
- Investor-facing risk and status disclosures

### Intentionally excluded

- Private source code, database schemas, migrations, CI internals, and infrastructure
- Threat-model details, security implementation notes, credentials, keys, or endpoints
- Customer, identity, asset, payment, compliance, or legal-document data
- Smart contracts, wallets, custody keys, token contracts, or blockchain configuration
- Real KYC/KYB, payment, Chainlink, Hedera, or other live integrations

## Security and contributions

Read [SECURITY.md](SECURITY.md) before reporting a security-sensitive concern. For documentation contributions, read [CONTRIBUTING.md](CONTRIBUTING.md) and the [website and documentation alignment guide](docs/product/website-and-docs-alignment.md).

Do not include credentials, private keys, identity documents, payment data, confidential legal material, customer data, or exploit details in public issues or pull requests.

## Important notice

Nothing in this repository constitutes legal, financial, investment, tax, accounting, or regulatory advice, or an offer, sale, solicitation, or recommendation involving securities, tokens, stable-value assets, or other financial instruments.
