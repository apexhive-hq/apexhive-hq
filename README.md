# ApexHive Labs

Open-Core MIT engineering lab building **AI agent context/security tooling (MCP & `x402`)**, **non-custodial Base USDC payment infrastructure**, and **self-hostable SME operations software**.

- **Showcase & Calculator:** [apexhive-showcase.pages.dev](https://apexhive-showcase.pages.dev)
- **Glama Directory:** [glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy](https://glama.ai/mcp/servers/apexhive-hq/slimmcp-proxy)
- **x402 Machine Discovery:** [`slimmcp-proxy` `.well-known/x402`](https://slimmcp-proxy-store.apexhive-hq.workers.dev/.well-known/x402) &bull; [`mcp-doctor` `.well-known/x402`](https://mcp-doctor-store.apexhive-hq.workers.dev/.well-known/x402)
- **Support & Recovery:** `apexhive.hq@proton.me`

---

## Public MIT Projects

| # | Project | What It Does | Source | Live App / Storefront |
|---:|---|---|---|---|
| 1 | **`slimmcp-proxy`** | Progressive-disclosure Meta-MCP proxy in pure Node.js (`>=24`) cutting initial `tools/list` context by up to `97.87%` via BM25 discovery, lazy schema load, and secret redaction + `$0.005` `x402` API (`npm: slimmcp-proxy`) | [GitHub (MIT)](https://github.com/apexhive-hq/slimmcp-proxy) | [Live Playground & Store](https://slimmcp-proxy-store.apexhive-hq.workers.dev) |
| 2 | **`zerofiat-base-checkout-kit`** | Non-custodial Base USDC (`eip155:8453`) checkout template on Cloudflare Workers + KV with a Cloud Hosted Verify API free for your first `$10,000 USDC` earned | [GitHub (MIT)](https://github.com/apexhive-hq/zerofiat-base-checkout-kit) | [Live Quota & Store](https://zerofiat-base-checkout-kit.apexhive-hq.workers.dev) |
| 3 | **`web3-ops-automation-pack`** | Open-source TypeScript & Python Base/Solana USDC payment verifiers, n8n webhook workflows, and Playwright Web3 QA harness | [GitHub (MIT)](https://github.com/apexhive-hq/web3-ops-automation-pack) | [Live Storefront](https://web3-ops-automation-pack-store.apexhive-hq.workers.dev) |
| 4 | **`mcp-doctor`** | MCP security & readiness auditor (CLI + Live GitHub Repo Scanner + dynamic SVG badges + `$0.005` `x402` deep audit API, `npm: apexhive-mcp-doctor`) | [GitHub (MIT)](https://github.com/apexhive-hq/mcp-doctor) | [Live Scanner & Store](https://mcp-doctor-store.apexhive-hq.workers.dev) |
| 5 | **`open-center-os` (`v2.1.0`)** | 6-View SME & Education Center ERP (full `node:sqlite` UI sync, 100% EN/繁中/簡中 i18n, `Teacher Roster`, `Parent Portal`, QR pass check-in, `Mark Paid`/`Void`/`Refund`, Timetable CRUD) | [GitHub (MIT)](https://github.com/apexhive-hq/open-center-os) | [Interactive 6-View Preview](https://open-center-os.apexhive-hq.workers.dev) |
| 6 | **`evalshield-copilot` (`v1.0.0`)** | Human-in-the-Loop Prop-Firm Risk & Discipline Firewall (zero order routing, zero broker API keys, `node:sqlite` WAL journal, 4 CSV adapters, 10k-run Monte Carlo) | [GitHub (MIT)](https://github.com/apexhive-hq/evalshield-copilot) | [Live Sim & Store](https://evalshield-copilot.apexhive-hq.workers.dev/) |

---

## Open-Source vs. Commercial Boundaries

All six repositories above are **100% MIT-licensed** and self-hostable from source with zero hidden telemetry or recurring SaaS lock-in:

- **Free & Unrestricted Under MIT (`0 USDC`):**
  - Run `slimmcp-proxy`, `mcp-doctor`, and `web3-ops-automation-pack` locally forever.
  - Self-host `zerofiat-base-checkout-kit` on your own Cloudflare Workers account forever (or use the Cloud Hosted Verify API free up to `$10,000 USDC` verified GMV).
  - Run `open-center-os` for **1 active branch** with full POS, CRM, timetable, QR check-in, and BI reporting at `$0` forever.
  - Run `evalshield-copilot` for **1 prop-firm evaluation account** locally (`node:sqlite` WAL + CSV adapters) at `$0` forever.
- **Optional Commercial Licenses & Voluntary Support (Non-Custodial Base USDC):**
  - **Voluntary Supporter / Patron Tiers (`5` / `15` / `49 USDC`):** Fund ongoing MIT maintenance and unlock signed Ed25519 policy/team guardrails (`slimmcp-proxy` Team `49 USDC`, `zerofiat` Hosted Pro past `$10k` GMV `49 USDC`).
  - **Prop-Firm Multi-Account & Monte Carlo (`evalshield-copilot`):** `29 USDC` Solo (up to 20 accounts + 10,000-run Monte Carlo) / `99 USDC` Team (unlimited accounts + read-only webhook ingest).
  - **Multi-Branch & Chain Licenses (`open-center-os`):** Creating `2–3` branches (`499 USDC` Team) or unlimited branches (`999 USDC` Chain) uses offline-verifiable Ed25519 license tokens.
  - **Pay-Per-Call `x402` Endpoints:** `$0.005 USDC` per call on `slimmcp-proxy` (`/api/x402/compress`) and `mcp-doctor` (`/api/x402/audit`) settled directly on Base Mainnet (`eip155:8453`) to `0x32eceaC45DBED9E555dAb80346aBd4Ab9C676206`.

---

## Quick Start (`npx`, GitHub Source, or Docker for Node 20/22)

Our CLI & server packages use Node.js `>=24` built-in `node:sqlite` (zero native C++ `node-gyp` dependencies). Run `slimmcp-proxy` (`v1.0.1`) or `apexhive-mcp-doctor` (`v1.0.0`) directly from npm, or build from GitHub:

```bash
# Instant run via npm (Node.js >= 24):
npx -y slimmcp-proxy --help
npx -y apexhive-mcp-doctor status

# Or build from GitHub source (includes 60-tool benchmark fixture):
git clone https://github.com/apexhive-hq/slimmcp-proxy.git
cd slimmcp-proxy/cli
pnpm install --ignore-scripts
pnpm run build
node dist/src/cli.js benchmark --config slimmcp.config.example.json
```

**On Node 20 / 22 hosts?** Run inside the official `node:24-slim` container (or use the included `Dockerfile` in `open-center-os`):

```bash
docker run --rm -v "$PWD:/app" -w /app/cli node:24-slim sh -c "npm i -g pnpm && pnpm install --ignore-scripts && pnpm run build && node dist/src/cli.js --help"
```
