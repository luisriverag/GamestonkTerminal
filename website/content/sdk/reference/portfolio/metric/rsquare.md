---
title: rsquare
description: Detailed information about using the 'rsquare' function in the 'openbb'
  portfolio metric, which calculates the R2 Score between a portfolio and a selected
  benchmark. The page includes examples of usage.
keywords:
- portfolio
- benchmark
- R2 Score
- PortfolioEngine
- openbb.portfolio.metric.rsquare
- openbb.portfolio.load
---

import HeadTitle from '@site/src/components/General/HeadTitle.tsx';

<HeadTitle title="portfolio.metric.rsquare - Reference | OpenBB SDK Docs" />

Get R2 Score for portfolio and benchmark selected

Source Code: [[link](https://github.com/OpenBB-finance/OpenBBTerminal/tree/main/openbb_terminal/portfolio/portfolio_model.py#L947)]

```python
openbb.portfolio.metric.rsquare(portfolio_engine: portfolio_engine.PortfolioEngine)
```

---

## Parameters

| Name | Type | Description | Default | Optional |
| ---- | ---- | ----------- | ------- | -------- |
| portfolio_engine | PortfolioEngine | PortfolioEngine class instance, this will hold transactions and perform calculations.<br/>Use `portfolio.load` to create a PortfolioEngine. | None | False |


---

## Returns

| Type | Description |
| ---- | ----------- |
| pd.DataFrame | DataFrame with R2 Score between portfolio and benchmark for different periods |
---

## Examples

```python
from openbb_terminal.sdk import openbb
p = openbb.portfolio.load("openbb_terminal/miscellaneous/portfolio_examples/holdings/example.csv")
output = openbb.portfolio.metric.rsquare(p)
```

---
