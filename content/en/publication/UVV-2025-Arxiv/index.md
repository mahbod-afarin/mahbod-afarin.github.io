---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Analysis of Stable Vertex Values: Fast Query Evaluation Over An Evolving Graph'
subtitle: ''
summary: ''
authors:
- Mahbod Afarin
- Chao Gao
- Xizhe Yin
- Zhijia Zhao
- Nael Abu-Ghazaleh
- Rajiv Gupta
tags: []
categories: []
date: '2025-02-14'
lastmod: 2025-02-14T19:57:59-04:00
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
publishDate: '2025-02-14T23:57:59.485338Z'
publication_types:
- '1'
abstract: '<div class="justify-text"> Evaluating a query over a large, irregular graph is inherently challenging. This challenge intensifies when solving a query over a sequence of snapshots of an evolving graph, where changes occur through the addition and deletion of edges. We carried out a study that shows that due to the gradually changing nature of evolving graphs, when a vertex-specific query (e.g., SSSP) is evaluated over a sequence of 25 to 100 snapshots, for 53.2% to 99.8% of vertices, the query results remain unchanged across all snapshots. Therefore, the Un- changed Vertex Values (UVVs) can be computed once and then minimal analysis can be performed for each snapshot to obtain the results for the remaining vertices in that snap- shot. We develop a novel intersection-union analysis that very accurately computes lower and upper bounds of vertex val- ues across all snapshots. When the lower and upper bounds for a vertex are found to be equal, we can safely conclude that the value found for the vertex remains the same across all snapshots. Therefore, the rest of our query evaluation is limited to computing values across snapshots for vertices whose bounds do not match. We optimize this latter step evaluation by concurrently performing incremental compu- tations on all snapshots over a significantly smaller subgraph. Our experiments with several benchmarks and graphs show that we need to carry out per snapshot incremental analysis for under 42% vertices on a graph with under 32% of edges. Our approach delivers speedups of 2.01-12.23× when com- pared to the state-of-the-art RisGraph implementation of the KickStarter-based incremental algorithm for 64 snapshots.
</div>'
publication: '*arXiv preprint arXiv:2502.10579*'
links:
- name: DOI
  url: https://arxiv.org/pdf/2502.10579
- name: PDF
  url: uploads/uvvArxiv.pdf
---


<style>
  .justify-text {
    text-align: justify;
  }
</style>
