---
# Documentation: https://wowchemy.com/docs/managing-content/

title: ' Sagas: Temporally Consistent Sampling of Evolving Graphs'
subtitle: ''
summary: ''
authors:
- Chao Gao
- Mahbod Afarin
- Xizhe Yin
- Nael Abu-Ghazaleh
- Rajiv Gupta
tags: []
categories: []
date: '2026-10-16'
lastmod: 2026-10-16T19:57:59-04:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2026-10-16T23:57:59.485338Z'
publication_types:
- '1'
abstract: '<div class="justify-text"> Graph sampling algorithms create a smaller representative subgraph by picking a subset of the vertices and edges of the original graph. Graph sampling has a wide range of applications including graph visualization, social network analysis, inductive learning, and graph sparsification. Substantial research has studied sampling algorithms for static graphs, using statistical sampling, random-walk-based approaches, data-driven approaches, and others, pursuing different goals with respect to the properties of the sample suitable for the desired application (we call preserving these desired properties the sample consistency goal of the sampling algorithm). Many graphs evolve over time, forming a series of graph snapshots, that analytics can use to answer temporal queries. However, if we apply static graph sampling on each snapshot independently, these samples will not represent a coherent temporal evolution and will be temporally inconsistent. In this work, we propose the first temporally-consistent dynamic graph sampling system. Starting from samples obtained using a traditional sampling algorithm on any one primary snapshot, we develop a sample-projection algorithm that projects samples to other snapshots, by repairing the samples if some of the edges in them do not exist in other snapshots. To measure temporal-consistency, we introduce new metrics including: (1) Structural Similarity metrics: changes in the samples of evolving snapshots reflect only changes in the original graph; and (2) Trend Divergence metrics: when measuring a property on the full evolving graph, the property should change in a corresponding direction on the sample. Our temporal sampling algorithm is computationally demanding for large graphs due to large overheads for projecting the samples. To address this cost, we develop a system that facilitates both primary graph sampling and efficient sample projection, enhanced by graph skeleton extraction, which allows sample projections to be repaired using a smaller skeleton graph. Our system, tested on six different graph types and two sampling algorithms, improves performance by nearly four orders of magnitude over sequential execution and improves temporal consistency by up to 99.1%.</div>'
publication: '*2026 IEEE International Conference on Big Data (BigData)* <span style="color:green;"> (Acceptance Rate: 19.4%) </span>'
links: []
---

<style>
  .justify-text {
    text-align: justify;
  }
</style>
