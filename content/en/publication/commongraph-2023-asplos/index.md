---
# Documentation: https://wowchemy.com/docs/managing-content/

title: ' CommonGraph: Graph Analytics on Evolving Data'
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
date: '2023-01-3301'
lastmod: 2023-01-18T19:57:59-04:00
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
publishDate: '2023-01-18T23:57:59.485338Z'
publication_types:
- '1'
abstract: '<div class="justify-text"> We consider the problem of graph analytics on evolving graphs (i.e., graphs that change over time). In this scenario, a query typically needs to be applied to different snapshots of the graph over an extended time window, for example to track the evolution of a property over time. Solving a query independently on multiple snapshots is inefficient due to repeated execution of subcomputation common to multiple snapshots. At the same time, we show that using streaming, where we start from the earliest snapshot and stream the changes to the graph incrementally updating the query results one snapshot at a time is also inefficient. We propose CommonGraph, an approach for efficient processing of queries on evolving graphs. We first observe that deletion operations are significantly more expensive than addition operations for many graph queries (those that are monotonic). CommonGraph converts all deletions to additions by finding a common graph that exists across all snapshots. After computing the query on this graph, to reach any snapshot, we simply need to add the missing edges and incrementally update the query results. CommonGraph also allows sharing of common additions among snapshots that require them, and breaks the sequential dependency inherent in the traditional streaming approach where snapshots are processed in sequence, enabling additional opportunities for parallelism. We incorporate the CommonGraph approach by extending the KickStarter streaming framework. We implement optimizations that enable efficient handling of edge additions without resorting to expensive in place graph mutations, significantly reducing the streaming overhead, and enabling direct reuse of shared edges among different snapshots. CommonGraph achieves 1.38x-8.17x improvement in performance over Kickstarter across multiple benchmarks.</div>'
publication: '*ASPLOS2023: Proceedings of the 28th ACM International Conference on Architectural Support for Programming Languages and Operating Systems, Volume 2* <span style="color:green;"> (Acceptance Rate: 26.66%) </span>'
links:
- name: DOI
  url: https://dl.acm.org/doi/10.1145/3575693.3575713
- name: PDF
  url: uploads/commongraph.pdf
- name: Video
  url: https://www.youtube.com/watch?v=1Kc7U9UWbao&t=9s
- name: Lightning Talk
  url: https://www.youtube.com/watch?v=FSY-fPiWIAs&list=PL9N8iVe1dFKneAz1HFsarlJoemzgg1IMO&index=8
---

<style>
  .justify-text {
    text-align: justify;
  }
</style>