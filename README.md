# ApexHive Labs

Independent engineering lab building **6 pure-free MIT developer & operations tools (`#1`–`#5` & `#7`)** plus **1 commercial flagship (`#6 evalshield-copilot`)**.

- **Showcase & Benchmark Calculator:** [apexhive-showcase.pages.dev](https://apexhive-showcase.pages.dev)
- **GitHub Portfolio (`@apexhive-hq`):** [github.com/apexhive-hq](https://github.com/apexhive-hq)
- **Official MCP Registry:** `io.github.apexhive-hq/slimmcp-proxy`
- **Glama MCP Directory:** [glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy](https://glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy)
- **Support:** `apexhive.hq@proton.me`

---

## Pure-Free MIT Tools (`#1`–`#5` & `#7`)

Every repository below is **100% free, unrestricted MIT open source** — zero license keys, zero gated tiers, and green CI.

| # | Project | What It Does & Runtime | Distribution & Links |
|---:|---|---|---|
| 1 | **`slimmcp-proxy`** (`v1.0.2`) | Progressive-disclosure Meta-MCP proxy (`Node >=22.13 LTS`; `stdio`, `Streamable-HTTP`, `SSE`) cutting 60-tool `tools/list` schemas from `60,185 -> 1,286` bytes (`97.86%` initial reduction: `15,047 -> 322` tok; **`~14,310` tok saved / `95.10%` net 1-turn; `~737` tok spent**), BM25 search, fail-closed secret redaction, isolated child env, and deny-overrides RBAC/budget guardrails | [GitHub (MIT)](https://github.com/apexhive-hq/slimmcp-proxy) &bull; `npx -y slimmcp-proxy --help` &bull; [Glama](https://glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy) |
| 2 | **`zerofiat-base-checkout-kit`** (`v2.1.0`) | Unlimited free Base Mainnet USDC (`eip155:8453`) verification rail on Cloudflare Workers (`Node >=22.18 LTS`) with scoped `TxClaimLockDO` isolation, EOA (`EIP-191`) + Smart Wallet (`ERC-1271` / `EIP-6492`) verification, and strict `409` anti-replay | [GitHub (MIT)](https://github.com/apexhive-hq/zerofiat-base-checkout-kit) &bull; [Reference Worker](https://zerofiat-base-checkout-kit.apexhive-hq.workers.dev) |
| 3 | **`web3-ops-automation-pack`** (`v1.0.1`) | Strict `BigInt` Base & `finalized` Solana USDC verifiers in TypeScript (`Node >=22.18 LTS`) and Python (`3.12+`), Playwright mock EIP-1193 checkout QA harness, and fail-closed HMAC-authenticated n8n webhook templates | [GitHub (MIT)](https://github.com/apexhive-hq/web3-ops-automation-pack) |
| 4 | **`mcp-doctor`** (`v1.0.1`) | Static regex security & context-tax MCP CLI linter (`Node >=20 LTS`; `A–F` grading, masked secret evidence, isolated stdio env, SARIF 2.1.0, `--policy`, `--ci`) | [GitHub (MIT)](https://github.com/apexhive-hq/mcp-doctor) &bull; `npx -y apexhive-mcp-doctor status` |
| 5 | **`open-center-os`** (`v2.2.0`) | **Self-Hosted SME ERP Module** (`Node >=24` for `node:sqlite`): multi-branch SME & education center ERP with `scrypt` password hashing, SQLite session revocation, trilingual UI (EN/繁中/簡中) & bilingual EN/ZH receipts, POS, timetable, QR check-in, and unlimited free branches | [GitHub (MIT)](https://github.com/apexhive-hq/open-center-os) |
| 7 | **`dmarczero`** (`v1.0.0`) | Zero-dependency DNS/DMARC/TLS anti-drift guard & streaming `RUA` aggregate analyzer (strictly rejects `RUF` forensic PII; `Node >=20 LTS` CLI / `>=22.13` BYO Worker) + authenticated self-hosted Cloudflare Email Worker + customizable white-label HTML report | [GitHub (MIT)](https://github.com/apexhive-hq/dmarczero) |

---

## Sole Commercial Flagship (`#6`)

| # | Project | What It Does & Licensing | Source & Cloud App |
|---:|---|---|---|
| 6 | **`evalshield-copilot`** (`v3.0.2`) | Strictly read-only rule-based cross-market futures & prop-firm risk shield (**ApexHive Dual Source-Available License**: `Solo 0 USDC Forever · Team Early-Bird 99 USDC · Enterprise Early-Bird 499 USDC`): Topstep/Apex/MFFU/FTMO/Tradeify presets, CME Futures (`ES/NQ/GC/CL`), Gold (`XAUUSD`), FX, Crypto Perps (`BTC/ETH/SOL` incl. `SOL-PERP`), verified `2026–2027` official Fed FOMC / BLS CPI / BLS NFP blackout schedule + US DST accuracy, `25,000`-run Monte Carlo, fail-closed BYO Cloudflare webhook, and DNS-validated IPv4/IPv6 SSRF protection. Zero broker API keys or automated order placement. | [GitHub (ApexHive Dual Source-Available License)](https://github.com/apexhive-hq/evalshield-copilot) &bull; [Hosted Cloud Flagship](https://evalshield-copilot.apexhive-hq.workers.dev/) |

---

## Quick Start

```bash
# 1. Progressive-disclosure Meta-MCP proxy (100% Free MIT, Node >=22.13 LTS)
npx -y slimmcp-proxy --help
npx -y slimmcp-proxy serve --config /abs/path/to/mcp-servers.json

# 2. Static MCP security & context-tax linter (100% Free MIT, Node >=20 LTS)
npx -y apexhive-mcp-doctor status

# 3. Clone & run verified 60-tool benchmark from source
git clone https://github.com/apexhive-hq/slimmcp-proxy.git
cd slimmcp-proxy/cli
pnpm install --ignore-scripts
pnpm run typecheck && pnpm test && pnpm run benchmark
```

---

## Policies & Support

- **Terms of Use:** [apexhive-showcase.pages.dev/terms.html](https://apexhive-showcase.pages.dev/terms.html)
- **Privacy (Zero Telemetry / Zero Cookies):** [apexhive-showcase.pages.dev/privacy.html](https://apexhive-showcase.pages.dev/privacy.html)
- **Commercial Refund Policy (`#6 EvalShield`):** [apexhive-showcase.pages.dev/refund.html](https://apexhive-showcase.pages.dev/refund.html)
- **Contact:** `apexhive.hq@proton.me`
