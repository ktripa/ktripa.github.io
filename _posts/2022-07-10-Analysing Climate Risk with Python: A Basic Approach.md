---
layout: post
title: "My First Climate Risk Analysis Post"
date: 2025-07-10 10:00:00 +0000
categories: [Climate Risk, Data Analysis]
---

# My First Climate Risk Analysis Post

## Introduction: Why Climate Risk Matters

Climate change is a huge challenge, and understanding its risks is vital. This is my very first step into exploring how data can help us understand these risks.

## My Simple Data Analysis

I used Python to look at some simulated temperature data. Here's a little bit of the code I used:

```python
import pandas as pd
import numpy as np

# Simulate some data
dates = pd.to_datetime(pd.date_range(start='1990-01-01', periods=360, freq='M'))
temperatures = 15 + np.random.normal(0, 2, 360) + np.linspace(0, 5, 360) # Simple warming trend
df = pd.DataFrame({'Date': dates, 'Temperature_C': temperatures})

print(df.head())
```

* **Important Note on the top part (`--- layout: post ... ---`):** This section is called "Front Matter." It's used by Static Site Generators (like Jekyll, which GitHub Pages uses by default) to add metadata to your post (title, date, categories). Even if you're not explicitly setting up Jekyll, including this is a good habit, and GitHub Pages will often process it.
* **Code Blocks (` ```python `):** To include code, you use three backticks (```) followed by the language name (e.g., `python`, `html`, `javascript`), then your code, and then three more backticks to close it. This gives you the nice syntax highlighting you saw in the Canvas.

