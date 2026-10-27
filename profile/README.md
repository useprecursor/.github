<div align="center">
  <h2>Precursor</h2>
  <p>Private company shares, issued as tokens on Robinhood Chain.</p>
  <p>
    <a href="https://useprecursor.xyz">Website</a> ·
    <a href="https://docs.useprecursor.xyz">Docs</a> ·
    <a href="https://useprecursor.xyz/explorer">Explorer</a> ·
    <a href="https://x.com/useprecursor">X</a>
  </p>
</div>

Most private companies still keep their cap table in a spreadsheet, and their shareholders have very few ways to sell before an exit. We think that can work a lot better.

Precursor lets a company put each of its share classes on-chain as a token. The company decides who can hold it, where they can be, how long they have to hold before selling, and when trading is allowed. Those rules are checked on every transfer, before anyone signs, and when a transfer is refused you get a clear reason code instead of a failed transaction.

On top of that, companies can run offerings, open Liquidity Windows so employees and early investors can sell at a fair clearing price, pay out distributions, hold votes and publish documents, all from one place.

## Repositories

| Repo | What's inside |
| :-- | :-- |
| [webapp](https://github.com/useprecursor/webapp) | The website, plus the Console for companies, the Portfolio for holders and the public Explorer |
| [contracts](https://github.com/useprecursor/contracts) | The share token, the rule modules, offerings, Liquidity Windows and the rest of the protocol, with tests and deploy scripts |
| [documentation](https://github.com/useprecursor/documentation) | The source for [docs.useprecursor.xyz](https://docs.useprecursor.xyz) |

## A few details

- Each share class is a single ERC-20 token with ERC-3643 style permissioned transfers.
- Rules are small modules a company switches on per class: region, eligibility, holding period, holder cap, trading windows, right of first refusal, ownership limits and vesting.
- Holdings are tracked by lot, so holding periods and vesting work the way they do on paper.
- We're live on Robinhood Chain testnet today, with mainnet next.

## Get in touch

If you're a company thinking about this, or you just want to poke at the contracts, we'd love to hear from you at [hello@useprecursor.xyz](mailto:hello@useprecursor.xyz). For security issues, please write to [security@useprecursor.xyz](mailto:security@useprecursor.xyz) instead of opening a public issue.
