---
title: oi
description: This page provides a detailed explanation on how to plot open interest
  using various parameters such as min, max, calls, and puts. It also includes usage
  examples.
keywords:
- Open interest
- Tutorial
- Parameters
- Option trading
---

import HeadTitle from '@site/src/components/General/HeadTitle.tsx';

<HeadTitle title="stocks/options/oi - Reference | OpenBB Terminal Docs" />

Plot open interest. Open interest represents the number of contracts that exist.

### Usage

```python
oi [-m MIN] [-M MAX] [-c] [-p]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| min | Min strike to plot | -1 | True | None |
| max | Max strike to plot | -1 | True | None |
| calls | Flag to plot call options only | False | True | None |
| puts | Flag to plot put options only | False | True | None |


---

## Examples

```python
2022 Feb 16, 09:13 (🦋) /stocks/options/ $ load SPY

2022 Feb 16, 09:14 (🦋) /stocks/options/ $ exp 10
Expiration set to 2022-03-11

2022 Feb 16, 09:14 (🦋) /stocks/options/ $ oi
```
![oi](https://user-images.githubusercontent.com/46355364/154282811-b8b7d36b-2e4e-44c0-8026-b244d97a8608.png)

---
