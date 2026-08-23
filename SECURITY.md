# Security policy — StrataMesh Laboratory

## Lab disclosure

StrataMesh Laboratory runs **experimental** infrastructure. It is **not** production mainnet, **not** aBFT-secure, and **not** a venue for real-value custody assumptions.

- Assume lab state can be reset.
- Do not deposit assets you cannot afford to lose.
- Cryptography labelled post-quantum is **placeholder** until the roadmap states otherwise.

## Reporting

Responsible disclosure for laboratory systems and public repositories:

1. Prefer private contact: **amcmorais@icloud.com** (operator AMCM ENI).
2. Do not open public issues for active exploitation paths against live lab endpoints until coordinated.
3. Include: affected component (worker / repo path / endpoint), reproduction steps, impact, and suggested severity.

## Scope

| In scope | Out of scope |
|----------|----------------|
| `stratamesh-core` protocol code and workers | Third-party upstream CF/GitHub platform bugs |
| Public lab endpoints on `*.calhegasmorais.pt` | Social engineering of the operator |
| Auth / clearance boundary mistakes | Issues requiring physical access to Fog hardware |

## Response

Reports are acknowledged as capacity allows. Fixes land in lab releases; there is no SLA on production severity because **there is no production mainnet**.
