# Website and documentation alignment

This guide defines how public Novera material should remain consistent across the website, GitHub organization profile, and repository documents.

## Source hierarchy

1. [Product status](https://noveraprotocol.org/status) — public capability-state summary
2. [Architecture overview](../architecture/overview.md) — public technical direction
3. [Product roadmap](roadmap.md) — planned sequence
4. [Public disclosures](../governance/public-disclosures.md) — token, stable-value, governance, and no-offer boundaries
5. [Status model](status-model.md) — vocabulary for claims

If two public statements conflict, stop and resolve the inconsistency before publishing another change.

## Contribution workflow

1. Open a narrowly scoped branch.
2. State which public source supports each changed product or integration claim.
3. Use the controlled status vocabulary.
4. Separate current MVP behavior from planned, evaluated, conditional, and excluded behavior.
5. Run a sensitive-data and unsupported-claims review.
6. Request review before merging.

## Content checks

- Use **Novera Protocol** as the public brand.
- Use the official slogan: **Your Assets, Your Control, Your Future.**
- Use the positioning: **Infrastructure for real-world assets.**
- Describe the product as pre-production.
- Describe the architecture as EVM-first and chain-agnostic.
- State that no production blockchain is selected.
- Describe Base only as a leading candidate under evaluation.
- Describe Hedera only as an optional future adapter.
- Describe Chainlink CRE, CCIP, and Proof of Reserve only as conditional future integrations.
- State that NovaID and NovaDeed use mock/synthetic behavior in the MVP.
- State that NOVA and NovaStable are not in the current MVP.

## Never publish

- Credentials, secrets, private keys, seed phrases, endpoints, or private infrastructure detail
- Real identity documents, payment data, customer data, asset data, or legal records
- Invented TVL, users, transactions, uptime, partners, audit status, or launch status
- Claims of legal finality, regulatory approval, production settlement, or active integration without evidence and authorization

## Pull-request description

Include:

- **Purpose** — why the public material needs to change
- **Evidence** — links to the governing source or approved decision
- **Status impact** — whether any capability label changes
- **Risk review** — security, legal, compliance, privacy, and brand considerations
- **Validation** — link, heading, accessibility, and formatting checks performed
