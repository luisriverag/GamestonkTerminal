---
title: tokens
description: Detailed guidance on displaying trade-able tokens on Uniswap DEX including
  parameters, usage, and examples. Useful for those interested in DeFi and cryptocurrency
  trading.
keywords:
- Uniswap DEX
- tokens
- cryptocurrency
- trading
- blockchain
- DeFi
- crypto trading
- tradeVolumeUSD
- totalLiquidity
- txCount
---

import HeadTitle from '@site/src/components/General/HeadTitle.tsx';

<HeadTitle title="crypto/defi/tokens - Reference | OpenBB Terminal Docs" />

Display tokens trade-able on Uniswap DEX [Source: https://thegraph.com/en/]

### Usage

```python
tokens [--skip SKIP] [--limit LIMIT] [-s {index,symbol,name,tradeVolumeUSD,totalLiquidity,txCount}] [-r]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| skip | Number of records to skip | 0 | True | range(1, 1000) |
| limit | Number of records to display | 20 | True | None |
| sortby | Sort by given column. Default: index | index | True | index, symbol, name, tradeVolumeUSD, totalLiquidity, txCount |
| reverse | Data is sorted in descending order by default. Reverse flag will sort it in an ascending way. Only works when raw data is displayed. | False | True | None |


---

## Examples

```python
2022 Feb 15, 06:36 (🦋) /crypto/defi/ $ tokens
                                 UniSwarp DEX Trade-able Tokens
┌───────┬──────────────┬────────────────────────────┬────────────────┬────────────────┬─────────┐
│ index │ symbol       │ name                       │ tradeVolumeUSD │ totalLiquidity │ txCount │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 0     │ BID          │ TopBidder                  │ 17.9M          │ 1.9M           │ 2496    │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 1     │ CHI          │ Chi Gastoken by 1inch      │ 19.4M          │ 25K            │ 75833   │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 2     │ XDEX         │ XDEFI Governance Token     │ 18.7M          │ 6.1M           │ 4316    │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 3     │ TUSD         │ TrueUSD                    │ 176.2M         │ 71.5K          │ 46582   │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 4     │ LON          │ Tokenlon                   │ 504M           │ 2.3M           │ 56107   │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 5     │ dDai         │ Dharma Dai                 │ 0              │ 4              │ 1       │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 6     │ STRIP        │ StripInu2                  │ 0              │ 0              │ 614     │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 7     │ GST2         │ Gastoken.io                │ 2.1M           │ 142            │ 10888   │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 8     │ XGME         │ GameStonk.online           │ 0              │ 35.7K          │ 65      │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 9     │ SHKOOBYSHNAX │ SHKOOBY INU SHNAX          │ 0              │ 0              │ 47      │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 10    │ PORN         │ Porn DAO                   │ 2.3M           │ 1.9K           │ 321     │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 11    │ TGBP         │ TrueGBP                    │ 24.1K          │ 4.1K           │ 740     │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 12    │ $STEALTH     │ Stealth Standard           │ 9.2M           │ 165.5M         │ 1622    │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 13    │ ADIDAS       │ Adidas Originals Metaverse │ 4.5M           │ 0              │ 488     │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 14    │ Nike         │ Nike RTFKT Studio          │ 75.8K          │ 0              │ 15      │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 15    │ DLTA         │ delta.theta                │ 3.1M           │ 2M             │ 2611    │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 16    │ Nike         │ Nike Metaverse             │ 4.5M           │ 0              │ 669     │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 17    │ Nike         │ Nike RTFKT Studio          │ 131.6K         │ 0              │ 35      │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 18    │ PRADA        │ Prada Metaverse            │ 894.8K         │ 0              │ 196     │
├───────┼──────────────┼────────────────────────────┼────────────────┼────────────────┼─────────┤
│ 19    │ TCAD         │ TrueCAD                    │ 6.5K           │ 599            │ 141     │
└───────┴──────────────┴────────────────────────────┴────────────────┴────────────────┴─────────┘
```
---
