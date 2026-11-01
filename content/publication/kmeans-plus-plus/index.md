---
title: Improved Guarantees for k-means++ and k-means++ Parallel
authors:
  - Konstantin Makarychev
  - admin
  - Liren Shan
author_notes:
  - Alphabetical ordering
  - Alphabetical ordering
  - Alphabetical ordering
date: 2020-12-14T01:00:00.000Z
publication_types:
  - "1"
publication: In *Advances in Neural Information Processing Systems 33 (NeurIPS 2020)*
publication_short: In *NeurIPS 2020* (CORE A\*)
abstract: In this paper, we study k-means++ and k-means||, the two most popular
  algorithms for the classic k-means clustering problem. We provide novel
  analyses and show improved approximation and bi-criteria approximation
  guarantees for k-means++ and k-means||. Our results give a better theoretical
  justification for why these algorithms perform extremely well in practice.
url_pdf: https://proceedings.neurips.cc/paper_files/paper/2020/file/ba304f3809ed31d0ad97b5a2b5df2a39-Paper.pdf
links:
  - name: arXiv
    url: https://arxiv.org/abs/2010.14487
  - name: Proceedings
    url: https://proceedings.neurips.cc/paper/2020/hash/ba304f3809ed31d0ad97b5a2b5df2a39-Abstract.html
---

k-means++ is the standard way to start k-means clustering and is the default in scikit-learn and MATLAB. Its scalable variant, the default in Apache Spark MLlib, often outperforms it, yet its known guarantees were much weaker. We improved the k-means++ guarantee from 8(ln k + 2) to 5(ln k + 2), gave sharper bi-criteria bounds, and proved new guarantees for the parallel variant.

Following the convention in theoretical computer science, authors are listed alphabetically and contributed equally.
