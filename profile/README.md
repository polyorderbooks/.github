# PolyOrderbooks

**Historical Polymarket order book API** — query archived L2 bid/ask depth, outcome prices, and liquidity metrics for crypto prediction markets.

Independent data product. Not affiliated with or endorsed by Polymarket.

## Links

| | URL |
|---|---|
| **Website** | https://polyorderbooks.com |
| **API** | https://api.polyorderbooks.com |
| **Documentation** | https://docs.polyorderbooks.com |
| **Quickstart** | https://docs.polyorderbooks.com/quickstart |
| **Sign up (free)** | https://polyorderbooks.com/signup |
| **Pricing** | https://polyorderbooks.com/pricing |

## What it does

PolyOrderbooks stores **historical** Polymarket market data so you can replay past order books — not just live snapshots or mid prices.

- **L2 order books** — bid/ask ladders as `[price, size]` per outcome
- **Prices & metrics** — outcome prices, volume, liquidity, spread on the same time window
- **Discovery** — search series, events, and markets (crypto coverage today)
- **Resolved markets** — settled markets stay queryable, including the winner
- **Read-local API** — your client calls our archive; read paths do not hit live Polymarket

Open markets are captured every second. Starter plans query down to **60s** resolution; Pro and Scale unlock **1s**.

## Quick example

```bash
export POLYORDERBOOKS_API_KEY="pob_your_key_here"

curl -s -H "X-API-Key: $POLYORDERBOOKS_API_KEY" \
  "https://api.polyorderbooks.com/v1/markets?search=bitcoin&limit=5"
```

Create a free API key: [polyorderbooks.com/signup](https://polyorderbooks.com/signup)

## Contact

- Email: [contact@polyorderbooks.com](mailto:contact@polyorderbooks.com)
- X: [@polyorderbooks](https://x.com/polyorderbooks)
