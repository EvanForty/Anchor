# ANCHOR

**Every coin needs an anchor.**

ANCHOR is a Solana launchpad for stock-backed coins. A creator launches a coin and picks a tokenized stock (NVDA, TSLA, SPY, AAPL and more). Part of every trading fee buys that stock into an on-chain reserve tied to the coin, and holders can burn coins to redeem a share of it.

This repository is the front end: one static page with no build step.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole site: markup, styles and script |
| `favicon.svg` | Browser tab icon |
| `README.md` | This file |

## Run locally

Open `index.html` in a browser. To serve it instead:

```bash
npx serve .
```

## Deploy to Vercel

1. Push these files to the root of a GitHub repository.
2. In Vercel, choose **Add New → Project** and import the repository.
3. Set **Framework Preset** to **Other**. Leave the build command and output directory empty.
4. Click **Deploy**.

## Before going live

- Stock prices are fixed values in the `STOCKS` array in `index.html`. Connect a price feed.
- The `COINS` array is empty. Load coins from the ANCHOR program on Solana.
- Wallet, launch, trade and redeem buttons show an "opens at launch" message. Wire them to a Solana wallet adapter and the program.
- Stock logos come from [Simple Icons](https://simpleicons.org) (CC0). Brand marks remain trademarks of their owners.
