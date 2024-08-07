---
# Documentation: https://wowchemy.com/docs/managing-content/

title: ' CommonGraph: Graph Analytics on Evolving Data (Abstract)'
subtitle: ''
summary: ''
authors:
- Mahbod Afarin
- Chao Gao
- Shafiur Rahman
- Nael Abu-Ghazaleh
- Rajiv Gupta
tags: []
categories: []
date: '2023-07-18'
lastmod: 2023-07-18T19:57:59-04:00
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
publishDate: '2023-07-18T23:57:59.485338Z'
publication_types:
- '1'
abstract: '<div class="justify-text"> We consider the problem of graph analytics on evolving graphs. In this scenario, a query typically needs to be applied to different snapshots of the graph over an extended time window. We propose CommonGraph, an approach for efficient processing of queries on evolving graphs. We first observe that edge deletions are significantly more expensive than addition operations. CommonGraph converts all deletions to additions by finding a common graph that exists across all snapshots. After computing the query on this graph, to reach any snapshot, we simply need to add the missing edges and incrementally update the query results. CommonGraph also allows sharing of common additions among snapshots that require them, and breaks the sequential dependency inherent in the traditional streaming approach where snapshots are processed in sequence, enabling additional opportunities for parallelism. We incorporate the CommonGraph approach by extending the KickStarter streaming framework. CommonGraph achieves 1.38x-8.17x improvement in performance over Kickstarter across multiple benchmarks.</div>'
publication: '*HOPC23: Proceedings of the 2023 ACM Workshop on Highlights of Parallel Computing*'
links:
- name: DOI
  url: https://dl.acm.org/doi/10.1145/3597635.3598022
- name: PDF
  url: uploads/commongraph_abstract.pdf
---

<style>
  .justify-text {
    text-align: justify;
  }
</style>