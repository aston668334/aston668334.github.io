---
layout: post
title: Manhattan 做圖
date: 2024-06-24 17:00:00
description: 簡單製作Manhattan圖
tags: Bioinformatic GWAS Manhattan-plot
categories: posts
code_diff: true
giscus_comments: true
---

# 曼哈頓圖簡介

曼哈頓圖是一種常用於基因組關聯研究（GWAS）結果可視化的方法。它將每個單核苷酸多態性（SNP）的 p 值在基因組中的位置進行展示，幫助研究人員快速識別與性狀或疾病顯著相關的基因變異。

## 常用的曼哈頓圖套件

1. [qqman](https://github.com/stephenturner/qqman)

   - **描述**：這是一個在 R 語言中開發的套件，提供了曼哈頓圖、Q-Q 圖和熱圖等圖表，同時支持基因注釋和功能注釋等功能。

2. [qmplot](https://github.com/ShujiaHuang/qmplot)

   - **描述**：這是一個在 Python 語言中開發的套件，提供了曼哈頓圖、Q-Q 圖，同時支持基因注釋和功能注釋等功能。

3. [PLINK](https://www.cog-genomics.org/plink/2.0/)

   - **描述**：這是一個開源軟件，支持線性迴歸分析、對照比分析和生存分析等，並提供了曼哈頓圖的繪製功能。

4. [Haploview](https://www.broadinstitute.org/haploview/haploview)

   - **描述**：這是一個用於基因型分析的軟件，同時也支持曼哈頓圖和 LD 圖等圖表，用於 GWAS 分析和遺傳分析。

5. [LocusZoom](https://my.locuszoom.org/)
   - **描述**：這是一個在線曼哈頓圖套件，可以用於對 GWAS 結果進行快速瀏覽和注釋，同時還支持基因注釋和 LD 計算等功能。

## 曼哈頓圖的特點

這些曼哈頓圖套件通常都提供了豐富的可定制化選項，例如顏色、標籤、字體等，可以讓用戶更好地呈現 GWAS 結果。需要注意的是，曼哈頓圖僅能用於快速展示 GWAS 結果，而不能進行詳細的統計分析和功能注釋。因此，在進行曼哈頓圖可視化時，還需進一步進行功能和統計分析。

![Manhattan Plot](/assets/img/blog/gwas-genome-wide-association-study_683773-52.avif)

_圖 1：典型的曼哈頓圖展示_

## 使用示例

### 使用 qqman 繪製曼哈頓圖

```r
# 安裝和加載 qqman 套件
install.packages("qqman")
library(qqman)

# 構建示例數據
set.seed(1234)
data <- data.frame(
  SNP = paste0("rs", 1:1000),
  CHR = rep(1:22, each = 50),
  BP = rep(1:50, times = 22),
  P = runif(1000, 0, 1)
)

# 繪製曼哈頓圖
manhattan(data)
```

### 使用 qmplot 繪製曼哈頓圖

```bash
# 安裝和加載 qmplot 套件
pip install qmplot
```

```python
import qmplot

# 構建示例數據
import pandas as pd
import numpy as np

np.random.seed(1234)
data = pd.DataFrame({
    'SNP': ['rs'+str(i) for i in range(1, 1001)],
    'CHR': np.repeat(np.arange(1, 23), 50),
    'BP': np.tile(np.arange(1, 51), 22),
    'P': np.random.uniform(0, 1, 1000)
})

# 繪製曼哈頓圖
qmplot.manhattanplot(data, chr='CHR', bp='BP', p='P')
```
