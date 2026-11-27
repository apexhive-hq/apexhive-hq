# ApexHive Labs

Local-first software for AI agent tooling, Web3 payment verification, multi-branch operations, email defense, and read-only trading risk analysis across four engineering areas.

- **Showcase & Context Calculator:** [apexhive-showcase.pages.dev](https://apexhive-showcase.pages.dev)
- **GitHub Portfolio (`@apexhive-hq`):** [github.com/apexhive-hq](https://github.com/apexhive-hq)
- **Official MCP Registry:** `io.github.apexhive-hq/slimmcp-proxy`
- **Glama MCP Directory:** [glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy](https://glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy)
- **Support:** `apexhive.hq@proton.me`

---

## AI Agent & MCP Tools

| Project | What It Solves | Links & License |
|---|---|---|
| **`slimmcp-proxy`** (`v1.0.3`) | Cuts 60-tool MCP schema context overhead by ~98% across `stdio`, Streamable-HTTP, and SSE upstreams (`Node >=22.13 LTS`). Exposes 3 meta-tools for BM25 discovery, lazy single-tool schema loading, secret redaction, and RBAC rules. | [GitHub](https://github.com/apexhive-hq/slimmcp-proxy) &bull; `npx -y slimmcp-proxy --help` &bull; [Glama](https://glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy) &bull; `MIT` |
| **`mcp-doctor`** (`v1.0.2`) | Static CI security and context-tax linter for MCP configs and JSON tool catalogs (`Node >=20 LTS`). Detects prompt injections, leaked secrets, bloated schemas, and policy violations with `A–F` grading and SARIF 2.1.0 output. | [GitHub](https://github.com/apexhive-hq/mcp-doctor) &bull; `npx -y apexhive-mcp-doctor status` &bull; `MIT` |

---

## Payments & Web3 Ops

| Project | What It Solves | Links & License |
|---|---|---|
| **`zerofiat-base-checkout-kit`** (`v2.1.0`) | Non-custodial Base Mainnet USDC payment verifier on Cloudflare Workers (`Node >=22.18 LTS`) with EOA + Smart Wallet (`ERC-1271` / `EIP-6492`) proofs, Durable Object anti-replay locks, and offline Ed25519 receipts. | [GitHub](https://github.com/apexhive-hq/zerofiat-base-checkout-kit) &bull; [Reference Worker](https://zerofiat-base-checkout-kit.apexhive-hq.workers.dev) &bull; `MIT` |
| **`web3-ops-automation-pack`** (`v1.0.1`) | Four verification and QA utilities (`Node >=22.18 LTS` / `Python 3.12+`): Base USDC watcher, `finalized` Solana SPL USDC verifier, Playwright EIP-1193 checkout QA harness, and HMAC-authenticated n8n webhooks. | [GitHub](https://github.com/apexhive-hq/web3-ops-automation-pack) &bull; `MIT` |

---

## Operations & Email Defense

| Project | What It Solves | Links & License |
|---|---|---|
| **`open-center-os`** (`v2.2.0`) | Self-hosted multi-branch ERP for schools, studios, and service centers (`Node >=24`, `node:sqlite`) with CRM trial leads, weekly timetables, QR check-in passes, POS invoicing, bilingual EN/ZH receipts, and `scrypt` session auth. | [GitHub](https://github.com/apexhive-hq/open-center-os) &bull; `MIT` |
| **`dmarczero`** (`v1.0.0`) | Zero-dependency DNS/DMARC/TLS anti-drift guard and streaming `RUA` aggregate analyzer (`Node >=20` CLI / `>=22.13` Worker; rejects `RUF` forensic PII), paired with an authenticated Cloudflare Email Worker and HTML reports. | [GitHub](https://github.com/apexhive-hq/dmarczero) &bull; `MIT` |

---

## Trading Risk Control

| Project | Capabilities & Licensing | Links |
|---|---|---|
| **`evalshield-copilot`** (`v3.0.2`) | **EvalShield Copilot — Read-Only Prop-Firm & Futures Risk Shield** (`Node >=24`). Six modules without broker API keys: **Drawdown Guard**, **Cross-Market Sizer**, **Portfolio Anti-Hedge Check**, **Trade Journal (`node:sqlite`)**, **Macro Event Calendar**, and **25k Monte Carlo & Alert Webhook**.<br />*License (ApexHive Dual Source-Available License):* Solo local use: Free · Team: `$99 USDC` · Enterprise: `$499 USDC`. | [GitHub](https://github.com/apexhive-hq/evalshield-copilot) &bull; [Web App](https://evalshield-copilot.apexhive-hq.workers.dev/) |

---

## Quick Start

```bash
# 1. Meta-MCP context proxy (Node >=22.13 LTS)
npx -y slimmcp-proxy --help
npx -y slimmcp-proxy serve --config /abs/path/to/mcp-servers.json

# 2. Static MCP security & context-tax linter (Node >=20 LTS)
npx -y apexhive-mcp-doctor status

# 3. Clone & run the 60-tool benchmark from source
git clone https://github.com/apexhive-hq/slimmcp-proxy.git
cd slimmcp-proxy/cli
pnpm install --ignore-scripts
pnpm run typecheck && pnpm test && pnpm run benchmark
```

---

## Policies & Support

- **Terms of Use:** [apexhive-showcase.pages.dev/terms.html](https://apexhive-showcase.pages.dev/terms.html)
- **Privacy (Zero Telemetry / Zero Cookies):** [apexhive-showcase.pages.dev/privacy.html](https://apexhive-showcase.pages.dev/privacy.html)
- **Refund Policy (EvalShield Copilot):** [apexhive-showcase.pages.dev/refund.html](https://apexhive-showcase.pages.dev/refund.html)
- **Contact:** `apexhive.hq@proton.me`
