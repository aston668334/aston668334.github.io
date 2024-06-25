---
layout: post
title: Manhattan 做圖
date: 2024-06-24 17:00:00
description: 簡單製作Manhattan圖
tags: Bioinformatic
categories: sample-posts
code_diff: true
giscus_comments: true
---

曼哈頓圖是一種常用於GWAS結果可視化的方法，常用的曼哈頓圖套件包括：

1. qqman: 這是一個在R語言中開發的套件，提供了曼哈頓圖、Q-Q圖和熱圖等圖表，同時支持基因注釋和功能注釋等功能。

2. PLINK: 這是一個開源軟件，提供了曼哈頓圖、Q-Q圖和LD圖等圖表，同時還支持線性迴歸分析、對照比分析和生存分析等。

3. Haploview: 這是一個用於基因型分析的軟件，同時也支持曼哈頓圖和LD圖等圖表，用於GWAS分析和遺傳分析。

4. LocusZoom: 這是一個在線曼哈頓圖套件，可以用於對GWAS結果進行快速瀏覽和注釋，同時還支持基因注釋和LD計算等功能。

這些曼哈頓圖套件通常都提供了豐富的可定制化選項，例如顏色、標籤、字體等，可以讓用戶更好地呈現GWAS結果。需要注意的是，曼哈頓圖僅能用於快速展示GWAS結果，而不能進行詳細的統計分析和功能注釋。因此，在進行曼哈頓圖可視化時，還需進一步進行功能和統計分析。



<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="/assets/img/blog/gwas-genome-wide-association-study_683773-52.avif" title="Manhattan_plot" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
