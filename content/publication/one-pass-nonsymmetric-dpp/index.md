---
title: One-Pass Algorithms for MAP Inference of Nonsymmetric Determinantal Point Processes
authors:
  - admin
  - Ryan A. Rossi
  - Zhao Song
  - Anup Rao
  - Tung Mai
  - Nedim Lipka
  - Gang Wu
  - Eunyee Koh
  - Nesreen Ahmed
author_notes:
  - Sole first and corresponding author
date: 2022-06-28T00:00:00.000Z
publication_types:
  - "1"
publication: In *Proceedings of the 39th International Conference on Machine Learning (ICML 2022)*
publication_short: In *ICML 2022* (CORE A\*)
url_pdf: https://proceedings.mlr.press/v162/reddy22a/reddy22a.pdf
links:
  - name: Proceedings
    url: https://proceedings.mlr.press/v162/reddy22a.html
---

Determinantal point processes are the standard probabilistic model of diverse subsets, used for example in recommender systems. Existing MAP inference algorithms for nonsymmetric DPPs must hold the whole dataset in memory, which is infeasible at industry scale. We started the study of streaming and online MAP inference for these models and designed one-pass algorithms that match the offline greedy algorithm using far less memory. We proved that no such algorithm has a worst-case guarantee, and gave one in the random-order model.

This work led to a [granted US patent](/publication/nonsymmetric-dpp-patent/) with Adobe Research. I am the sole first and corresponding author.
