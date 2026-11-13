# Satoshi Shell

A browser-based Bitcoin command-line simulator. Run `bitcoin-cli`-style commands and see how anyone can audit the Bitcoin network with simple, open tools.

**Live demo:** https://jon-hodl.github.io/Satoshi-Shell/

## Why we created this

Most people think auditing Bitcoin means trusting a company, reading a headline, or running a full node. Satoshi Shell shows that the same commands a Bitcoin node uses are understandable and verifiable by anyone — no special hardware required.

Type a command, click a question, or just read the output. The goal is to remove the mystery and leave you with one belief: **you do not have to trust anyone to verify Bitcoin.**

## What it does

- Answers common Bitcoin questions with real commands:
  - What is the total supply of Bitcoin?
  - What is the current block height?
  - How busy is the mempool?
  - What is the network hashrate?
- Fetches live data from [mempool.space](https://mempool.space), a community-run Bitcoin explorer.
- Explains every command and result in plain language.
- Works as a single standalone HTML file — no build step, no dependencies.

## Supported commands

| Command | What it shows |
|---------|---------------|
| `getblockcount` | Current block height |
| `getbestblockhash` | Hash of the latest block |
| `gettxoutsetinfo` | Total issued BTC (estimate) |
| `getmempoolinfo` | Pending transactions and fees |
| `getnetworkhashps` | Network hashrate |
| `getdifficulty` | Mining difficulty (estimate) |
| `getblockchaininfo` | Chain status overview |
| `estimatesmartfee` | Fee estimate for next block |

## How to use

1. Open `index.html` in any modern browser, or visit the live demo.
2. Type a command and hit **Run**, or click one of the question cards.
3. Read the command output and the plain-English explanation below it.

## Data source

All live Bitcoin data comes from the mempool.space API. No API key is required. Commands that require a full node are clearly labeled as estimates and include a note on how to verify them with your own node.

## License

MIT — see [LICENSE](./LICENSE).

---

Made with 🧨 by bitcoiners (Jon & Finn) for bitcoiners.
