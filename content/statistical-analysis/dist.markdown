---
title: Document/feature similarity
weight: 30
chapter: false
draft: false
---


```r
require(quanteda)
```

`textstat_dist()` calcuates similarites of documents or features for various measures. Its output is compatible with R's `dist()`, so hierachical clustering can be perfromed without any transformation.


```r
toks_inaug <- tokens(data_corpus_inaugural)
dfmat_inaug <- dfm(toks_inaug, remove = stopwords('en'))
tstat_dist <- textstat_dist(dfmat_inaug)
clust <- hclust(tstat_dist)
plot(clust, xlab = "Distance", ylab = NULL)
```

<img src="/statistical-analysis/dist_files/figure-html/unnamed-chunk-2-1.png" width="960" />


