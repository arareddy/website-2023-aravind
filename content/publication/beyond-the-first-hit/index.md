---
title: "Beyond the First Hit: Towards Tight Guarantees for k-means++"
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

k-means++ is the standard way to start k-means clustering. Its worst-case approximation ratio was known to be at most 8(ln k + 2), improved to 5(ln k + 2) in our [NeurIPS 2020 paper](/publication/kmeans-plus-plus/). We lower the leading coefficient of ln k from 5 to 2.108 with a computer-assisted proof, and give a short analytic proof with coefficient 2.3139. We also determine the exact ratio for two and three clusters, and prove new lower bounds.

Our key idea is to follow how a cluster's cost changes after it is first sampled. Earlier analyses charged that cost for the rest of the run, but a cluster left with a large cost is likely to be sampled again soon, which repairs it.
