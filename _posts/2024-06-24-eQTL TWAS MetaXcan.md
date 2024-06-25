---
layout: post
title: eQTL TWAS MetaXcan
date: 2024-06-24 17:00:00
description: eQTL TWAS MetaXcan 簡介
tags: Bioinformatic MetaXcan eQTL TWAS
categories: posts
code_diff: true
giscus_comments: true
---
轉錄體全基因結合研究（TWAS）是一種結合基因資料和基因表達信息的方法，用於研究基因表達與複雜性狀或疾病之間的關係。通過分析特定組織的基因表達，TWAS可以更有針對性和特定性地調查基因-狀態關聯。相比傳統的GWAS，TWAS擁有更低的多重檢驗負擔，可以幫助鑒定複雜表型的潛在致病基因。因此，TWAS已經成為遺傳流行病學中的一種熱門工具，用於發現與疾病相關的新基因關聯。


<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="/assets/img/blog/Principles-of-eQTL-mapping-for-investigating-immune-response-variation-A-General.png" title="Principles-of-eQTL-mapping-for-investigating-immune-response-variation-A-General" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

MetaXcan是一種統計方法，用於整合轉錄組和基因組學數據，以預測表型的基因表達量。它使用基因表達量的調節模式，即外源SNP對目標基因的影響，來計算每個基因的表達量。 MetaXcan的主要優勢在於，它可以在相對較小的樣本數據集中進行基因表達量預測，並且可以利用大型轉錄組和基因組學數據庫來獲得更高的預測能力。它還可以用於識別表型的潛在遺傳基礎和疾病發生機制的新穎生物學標誌物，例如高血壓。

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="/assets/img/blog/F2.large.jpg
" title="F2.large" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
