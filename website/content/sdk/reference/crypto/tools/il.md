---
title: il
description: 'This page provides technical documentation for two imperative features
  in OpenBB''s cryptocurrency tool suite: the Impermanent Loss calculation model and
  its corresponding chart display. Learn about their parameters, return types, and
  source code.'
keywords:
- Cryptocurrency
- Impermanent Loss
- Impermanent Loss Model
- Impermanent Loss Chart Display
- Crypto Tool Suite
- Crypto A
- Crypto B
- Liquidity Pool
---

import HeadTitle from '@site/src/components/General/HeadTitle.tsx';

<HeadTitle title="crypto.tools.il - Reference | OpenBB SDK Docs" />

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
<TabItem value="model" label="Model" default>

Calculates Impermanent Loss in a custom liquidity pool

Source Code: [[link](https://github.com/OpenBB-finance/OpenBBTerminal/tree/main/openbb_terminal/cryptocurrency/tools/tools_model.py#L57)]

```python
openbb.crypto.tools.il(price_changeA: float, price_changeB: float, proportion: float, initial_pool_value: float)
```

---

## Parameters

| Name | Type | Description | Default | Optional |
| ---- | ---- | ----------- | ------- | -------- |
| price_changeA | float | price change of crypto A in percentage | None | False |
| price_changeB | float | price change of crypto B in percentage | None | False |
| proportion | float | percentage of first token in pool | None | False |
| initial_pool_value | float | initial value that pool contains | None | False |


---

## Returns

| Type | Description |
| ---- | ----------- |
| Tuple[pd.DataFrame, str] | - pd.DataFrame: dataframe with results<br/>- str: narrative version of results |
---

</TabItem>
<TabItem value="view" label="Chart">

Displays Impermanent Loss in a custom liquidity pool

Source Code: [[link](https://github.com/OpenBB-finance/OpenBBTerminal/tree/main/openbb_terminal/cryptocurrency/tools/tools_view.py#L56)]

```python
openbb.crypto.tools.il_chart(price_changeA: int, price_changeB: int, proportion: int, initial_pool_value: int, narrative: bool = False, export: str = "")
```

---

## Parameters

| Name | Type | Description | Default | Optional |
| ---- | ---- | ----------- | ------- | -------- |
| price_changeA | float | price change of crypto A in percentage | None | False |
| price_changeB | float | price change of crypto B in percentage | None | False |
| proportion | float | percentage of first token in pool | None | False |
| initial_pool_value | float | initial value that pool contains | None | False |
| narrative | str | display narrative version instead of dataframe | False | True |
| export | str | Export dataframe data to csv,json,xlsx file |  | True |


---

## Returns

This function does not return anything

---

</TabItem>
</Tabs>
