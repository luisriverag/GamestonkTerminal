---
title: stat
description: This page provides a comprehensive guide on how to use two functions,
  stat and chart, in the OpenBBTerminal for COVID-19 data analysis. They are used
  for retrieving and visualising historical cases and deaths by country.
keywords:
- stat function
- chart function
- COVID-19 data analysis
- historical cases and deaths
- Country-wise data
- Data visualisation
- pandas DataFrame
---

import HeadTitle from '@site/src/components/General/HeadTitle.tsx';

<HeadTitle title="alt.covid.stat - Reference | OpenBB SDK Docs" />

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
<TabItem value="model" label="Model" default>

Show historical cases and deaths by country.

Source Code: [[link](https://github.com/OpenBB-finance/OpenBBTerminal/tree/main/openbb_terminal/alternative/covid/covid_model.py#L136)]

```python
openbb.alt.covid.stat(country: str, stat: str = "cases", limit: int = 10)
```

---

## Parameters

| Name | Type | Description | Default | Optional |
| ---- | ---- | ----------- | ------- | -------- |
| country | str | Country to get data for | None | False |
| stat | str | Statistic to get.  Either "cases", "deaths" or "rates" | cases | True |
| limit | int | Number of raw data to show | 10 | True |


---

## Returns

| Type | Description |
| ---- | ----------- |
| pd.DataFrame | Dataframe of data for given country and statistic |
---

</TabItem>
<TabItem value="view" label="Chart">

Prints table showing historical cases and deaths by country.

Source Code: [[link](https://github.com/OpenBB-finance/OpenBBTerminal/tree/main/openbb_terminal/alternative/covid/covid_view.py#L172)]

```python
openbb.alt.covid.stat_chart(country: str, stat: str = "cases", raw: bool = False, limit: int = 10, export: str = "", plot: bool = True)
```

---

## Parameters

| Name | Type | Description | Default | Optional |
| ---- | ---- | ----------- | ------- | -------- |
| country | str | Country to get data for | None | False |
| stat | str | Statistic to get.  Either "cases", "deaths" or "rates" | cases | True |
| raw | bool | Flag to display raw data | False | True |
| limit | int | Number of raw data to show | 10 | True |
| export | str | Format to export data |  | True |
| plot | bool | Flag to plot data | True | True |


---

## Returns

This function does not return anything

---

</TabItem>
</Tabs>
