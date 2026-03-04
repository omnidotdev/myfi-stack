# MyFi Stack

Unified asset management, portfolio tracking, and accounting.

## Modules

- **Books** — Multi-entity financial management (business + personal)
- **Ledger** — Double-entry journal entries with hierarchical chart of accounts
- **Budgets** — Budget rules, tracking, and alerts
- **Crypto** — Wallet connections, DeFi, NFTs, cost-basis engine
- **Reports** — P&L, balance sheet, cash flow, tax reports

## Architecture

| Service | Description | Port |
|---------|-------------|------|
| myfi-db | PostgreSQL 16 | 5432 |
| myfi-api | Elysia + PostGraphile | 4000 |
| myfi-app | TanStack Start | 3000 |

## Development

```bash
# Start services
docker compose -f compose.dev.yaml up

# Or use Weaver
weaver up
```
