---
title: "The Approximation Ratio of k-means++ Is 2 ln k + O(1)"
authors:
  - admin
date: 2026-11-09T00:00:00.000Z
publication_types:
  - "3"
publication: arXiv preprint arXiv:2611.14573
publication_short: arXiv preprint
url_pdf: https://arxiv.org/pdf/2611.14573
links:
  - name: arXiv
    url: https://arxiv.org/abs/2611.14573
---

k-means++ is the standard way to start k-means clustering. Its worst-case approximation ratio was known to be at least 2 ln k and at most 8(ln k + 2), and our [NeurIPS 2020 paper](/publication/kmeans-plus-plus/) improved the upper bound to 5(ln k + 2). We prove that the ratio is 2 ln k + O(1): for every k ≥ 2 it lies between 2H<sub>k−1</sub> + 2 and 2H<sub>k−2</sub> + 5, where H<sub>j</sub> is the j-th harmonic number, so the two bounds differ by less than 3. We also determine the exact ratio for two and three clusters, and give a second family of lower bounds that is stronger for small k.

Our key idea is to follow how a cluster's cost changes after it is first sampled. At each later draw, the chance of sampling the cluster again is exactly its share of the current cost, and we show that the cost reductions from these later hits bring the leading coefficient down to 2.
