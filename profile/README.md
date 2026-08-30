## StrataMesh Laboratory

Research DLT for **Fog/Edge resource coordination** and **STRATA settlement**.

**LAB** — not mainnet · not aBFT · PQ placeholders only.

**Open contribution.** Fork any public repo → PR to `main`. `@amcmorais` is **one contributor** (org admin / reference-node operator via AMCM ENI), not a personal mainline.
**Subject–Object Economy:** humans and SCAs are **subjects**; STRATA/NFTs/resources are **objects**. Population = subjects only. [Normative note](https://github.com/StrataMesh-Laboratory/stratamesh-core/blob/main/docs/SUBJECT-OBJECT-ECONOMY.md).

| Repository | Role |
|------------|------|
| [stratamesh-core](https://github.com/StrataMesh-Laboratory/stratamesh-core) | Protocol core — DAG, gossip, tip selection, STRATA, workers |
| [stratamesh-laboratory](https://github.com/StrataMesh-Laboratory/stratamesh-laboratory) | Lab charter, posture, research focus, ladder |
| [calhegas-morais-node](https://github.com/StrataMesh-Laboratory/calhegas-morais-node) | Reference Fog Node `FOG-NODE-PT-CM-001` (Lisboa) |
| [stratamesh-impact-fund](https://github.com/StrataMesh-Laboratory/stratamesh-impact-fund) | Pooled grants · challenges · Sponsors rails ([fund.calhegasmorais.pt](https://fund.calhegasmorais.pt/)) |

**Start here:** [CONTRIBUTING.md](https://github.com/StrataMesh-Laboratory/.github/blob/main/CONTRIBUTING.md) · [Impact challenges](https://fund.calhegasmorais.pt/challenges) · [Security](https://github.com/StrataMesh-Laboratory/stratamesh-core/blob/main/SECURITY.md)

**Archived personal path:** [`amcmorais/stratamesh-core`](https://github.com/amcmorais/stratamesh-core) is outdated — use the org core only.

**Operator entity:** [AMCM ENI](https://github.com/amcmorais/amcm-eni) · **Site:** [calhegasmorais.pt](https://calhegasmorais.pt/) · **Status:** [status.calhegasmorais.pt](https://status.calhegasmorais.pt/)

**Forum:** [stratamesh.discourse.group](https://stratamesh.discourse.group) · Contact: `geral@eni.calhegasmorais.pt`

### Install a node (lab)

Latest trees are on **[v0.4.2-lab](https://github.com/StrataMesh-Laboratory/stratamesh-core/releases/tag/v0.4.2-lab)**. The Fog **kit** shipped as **[v0.3.0](https://github.com/StrataMesh-Laboratory/stratamesh-core/releases/tag/v0.3.0)**. Lab prereleases. Not mainnet. `oracle_live=false`. `f_max=0` until n≥3.

| Node | Substrate | Release | Installer |
|------|-----------|---------|-----------|
| **Fog** | macOS | [v0.3.0 kit](https://github.com/StrataMesh-Laboratory/stratamesh-core/releases/tag/v0.3.0) · tree [v0.4.2-lab](https://github.com/StrataMesh-Laboratory/stratamesh-core/tree/v0.4.2-lab/deploy/mac-fog) | Double-click [`FogNodeInstaller.command`](https://github.com/StrataMesh-Laboratory/stratamesh-core/blob/v0.4.2-lab/deploy/mac-fog/FogNodeInstaller.command) or `python3 deploy/mac-fog/fog-bootstrap.py`. Finder apps: [`deploy/mac-fog/apps/`](https://github.com/StrataMesh-Laboratory/stratamesh-core/tree/v0.4.2-lab/deploy/mac-fog/apps). Kit notes: [`deploy/fog-node/README.md`](https://github.com/StrataMesh-Laboratory/stratamesh-core/blob/v0.4.2-lab/deploy/fog-node/README.md). |
| **Edge** | iOS (iPhone / iPad) | kit **v0.3.1** on tree [v0.4.2-lab](https://github.com/StrataMesh-Laboratory/stratamesh-core/tree/v0.4.2-lab/deploy/ios-edge) | **PWA now:** [api-edge.calhegasmorais.pt/app/](https://api-edge.calhegasmorais.pt/app/) → Share → Add to Home Screen. Native: open [`deploy/ios-edge/StrataMeshEdge/`](https://github.com/StrataMesh-Laboratory/stratamesh-core/tree/v0.4.2-lab/deploy/ios-edge/StrataMeshEdge) in Xcode 15+, team-sign, Run on device. Notes: [`deploy/ios-edge/README.md`](https://github.com/StrataMesh-Laboratory/stratamesh-core/blob/v0.4.2-lab/deploy/ios-edge/README.md). |

Request a `FOG-NODE-…` or `EDGE-NODE-…` id on [Discourse](https://stratamesh.discourse.group) first (bound to the operator email). Wizard is 2FA. No secrets in git.

**CMN MacBook continuity (why public Fog drops):** the reference origin is the laptop — named tunnel → workerd `:8788` → Fog `:8787`, `ORIGIN=macbook`. Sleep / lid / battery **halts the CPU**. That is not a Fog crash; cloudflared and workerd are off, so the public origin goes dark. Idle-sleep is held by [`FogStayAwake.command`](https://github.com/StrataMesh-Laboratory/stratamesh-core/blob/v0.4.2-lab/deploy/mac-fog/FogStayAwake.command) (`caffeinate -ims` + 2 min wake kick). **Lid + battery still sleeps (hardware).** On charger, lid-closed stay-up is `sudo pmset -c disablesleep 1`. Edge continuity is **session** by design (`C_mesh = f(1−U)`).

### Holonic stack (lab)

```
TRD StrataMesh
  └ Fog Node (FOG-NODE-PT-CM-001)
      └ SO Metaverso → Domínio Virtual → Mundo Aberto → Bancada CGU → Utilizador | SCA
```

`#mint` emits via Proof of Contribution · wallets circulate · `#0` burns.

### Normative drafts (core)

- [`docs/WIRE-PROTOCOL-v1.md`](https://github.com/StrataMesh-Laboratory/stratamesh-core/blob/main/docs/WIRE-PROTOCOL-v1.md)
- [`docs/THREAT-MODEL-v1.md`](https://github.com/StrataMesh-Laboratory/stratamesh-core/blob/main/docs/THREAT-MODEL-v1.md)
- [`src/protocol_benchmark.py`](https://github.com/StrataMesh-Laboratory/stratamesh-core/blob/main/src/protocol_benchmark.py)

**Contributors:** problem tracks for libp2p / edge / compute-economy / agents / worlds engineers — [outreach map](https://github.com/StrataMesh-Laboratory/stratamesh-core/blob/main/docs/COMMUNITY-OUTREACH-MAP.md) · [Fund challenges](https://fund.calhegasmorais.pt/challenges).
