# Contributing — StrataMesh Laboratory

## Where code lives

| Work | Repository |
|------|------------|
| Protocol, workers, benchmarks, wire/threat docs | [stratamesh-core](https://github.com/StrataMesh-Laboratory/stratamesh-core) |
| Lab posture, charter, research framing | [stratamesh-laboratory](https://github.com/StrataMesh-Laboratory/stratamesh-laboratory) |
| Reference Fog Node identity & ops registry | [calhegas-morais-node](https://github.com/StrataMesh-Laboratory/calhegas-morais-node) |

## Principles

1. **Subtraction over addition** — protocol invariants before metaverse surface area.
2. **Lab honesty** — never claim mainnet, aBFT finality, or production PQ.
3. **Normative docs first** — behaviour that contradicts `WIRE-PROTOCOL-v1` / `THREAT-MODEL-v1` is a bug or a doc PR, not silent drift.
4. **Economic poles** — `#mint` emit-only (PoC); `#0` burn-only; Fog `NODE_WALLET` is treasury, not a user/SCA account.

## Practical path

```bash
git clone https://github.com/StrataMesh-Laboratory/stratamesh-core.git
cd stratamesh-core/src && python3 protocol_benchmark.py
```

Open PRs against `main` with: what changed, which invariant or scenario it touches, and lab risk if any.

## Holonic vocabulary (do not collapse)

`TRD ≠ Fog Node ≠ SO Metaverso ≠ Domínio Virtual ≠ Mundo Aberto ≠ Bancada CGU ≠ Utilizador|SCA`

Forbidden shorthand that merges host OS / VM / Metaverse OS into one bag.
