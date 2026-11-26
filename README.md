# ApexHive Labs

Independent open-source engineering lab building **5 pure-free MIT developer & operations tools** (MCP context/security tooling, Base USDC verification rails, and self-hostable SME software) plus **1 hosted cloud risk flagship (`evalshield-copilot`)**.

- **Showcase & Benchmark Calculator:** [apexhive-showcase.pages.dev](https://apexhive-showcase.pages.dev)
- **Official MCP Registry:** `io.github.apexhive-hq/slimmcp-proxy`
- **Glama MCP Directory:** [glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy](https://glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy)
- **Support:** `apexhive.hq@proton.me`

---

## Pure-Free MIT Tools (`#1`–`#5`)

Every repository below is **100% free, unrestricted MIT open source** — zero license keys, zero gated tiers, and green GitHub Actions CI (`Node.js >= 24` / `Python 3.12+`).

| # | Project | What It Does | Distribution & Links |
|---:|---|---|---|
| 1 | **`slimmcp-proxy`** (`v1.0.2`) | Progressive-disclosure Meta-MCP proxy (`stdio`, `Streamable-HTTP`, `SSE`) in pure Node.js (`>=24`) replacing bloated `tools/list` definitions with 3 meta-tools (`97.86%` initial schema reduction: `60,185 -> 1,286` B across 60 tools; **`~737` tok / `~95.1%` net 1-turn savings**), BM25 search, secret redaction, and free RBAC/budget guardrails | [GitHub (MIT)](https://github.com/apexhive-hq/slimmcp-proxy) &bull; `npx -y slimmcp-proxy --help` &bull; [Glama](https://glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy) |
| 2 | **`zerofiat-base-checkout-kit`** (`v2.1.0`) | Non-custodial Base Mainnet USDC (`eip155:8453`) verification rail on Cloudflare Workers + SQLite Durable Object atomic anti-replay lock (`TxClaimLockDO`) with EOA (`EIP-191`) and Smart Wallet (`ERC-1271` / `EIP-6492`) signature verification | [GitHub (MIT)](https://github.com/apexhive-hq/zerofiat-base-checkout-kit) &bull; [Reference Worker](https://zerofiat-base-checkout-kit.apexhive-hq.workers.dev) |
| 3 | **`web3-ops-automation-pack`** | Cross-platform TypeScript (`Node.js >= 24`) and Python (`3.12+`) Base/Solana USDC payment verifiers, Playwright mock EIP-1193 checkout QA harness, and n8n webhook templates | [GitHub (MIT)](https://github.com/apexhive-hq/web3-ops-automation-pack) |
| 4 | **`mcp-doctor`** (`v1.0.1`) | Lightweight static regex-based MCP security & context-tax CLI linter (`A–F` grading, secret/injection pattern rules, `--policy`, `--ci --min-score`, SARIF 2.1.0) | [GitHub (MIT)](https://github.com/apexhive-hq/mcp-doctor) &bull; `npx -y apexhive-mcp-doctor status` |
| 5 | **`open-center-os`** (`v2.2.0`) | Multi-branch SME & education center ERP (`node:sqlite`, trilingual EN/繁中/簡中 UI, `HttpOnly` HMAC cookie + Bearer admin auth, locked CORS, POS cart, timetable, QR pass check-in, unlimited free branches) | [GitHub (MIT)](https://github.com/apexhive-hq/open-center-os) |

---

## Hosted Cloud Flagship (`#6`)

| # | Project | What It Does | Source & Cloud App |
|---:|---|---|---|
| 6 | **`evalshield-copilot`** | Human-in-the-loop futures & prop-firm evaluation risk shield (`INTRADAY_TRAILING`, `EOD_TRAILING`, `STATIC`, 8 CME contracts + micro fallbacks, 4 broker CSV adapters, `node:sqlite` WAL, 10,000-run Monte Carlo). Strictly read-only: **zero broker API keys and zero automated order placement.** | [GitHub (MIT Core)](https://github.com/apexhive-hq/evalshield-copilot) &bull; [Hosted Cloud Flagship](https://evalshield-copilot.apexhive-hq.workers.dev/) |

---

## Quick Start (`Node.js >= 24`)

Run the MCP CLI tools directly with `npx` or clone and test any repository from source:

```bash
# 1. Progressive-disclosure Meta-MCP proxy (100% Free MIT)
npx -y slimmcp-proxy --help
npx -y slimmcp-proxy serve --config /abs/path/to/mcp-servers.json

# 2. Static MCP security & context-tax linter (100% Free MIT)
npx -y apexhive-mcp-doctor status

# 3. Clone & run verified 60-tool benchmark from source
git clone https://github.com/apexhive-hq/slimmcp-proxy.git
cd slimmcp-proxy/cli
pnpm install --ignore-scripts
pnpm run typecheck && pnpm test && pnpm run benchmark
```

---

## Internal R&D (`polymarket-paper`)

Alongside our public developer repositories, we maintain an internal read-only `$0`-capital research engine (`polymarket-paper`) with a SHA-256 hash-chained simulation ledger and Brier calibration benchmarks. It operates strictly as zero-capital R&D and is not a public investment or custody product.

---

If our open-source tools saved your team time or tokens, voluntary Base USDC tips are welcome at `0x32eceaC45DBED9E555dAb80346aBd4Ab9C676206`.
