---
# Documentation: https://wowchemy.com/docs/managing-content/

title: ' Core Graph: Exploiting Edge Centrality to Speedup the Evaluation of Iterative Graph Queries'
subtitle: ''
summary: ''
authors:
- Xiaolin Jiang
- Mahbod Afarin
- Zhijia Zhao
- Nael Abu-Ghazaleh
- Rajiv Gupta
tags: []
categories: []
date: '2024-4-22'
lastmod: 2024-04-18T19:57:59-04:00
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
publishDate: '2024-04-18T23:57:59.485338Z'
publication_types:
- '1'


abstract: '<div class="justify-text"> When evaluating an iterative graph query over a large graph, systems incur significant overheads due to repeated graph transfer across the memory hierarchy coupled with repeated (redundant) propagation of values over the edges in the graph. An approach for reducing these overheads combines the use of a small proxy graph and the large original graph in a two phase query evaluation. The first phase evaluates the query on the proxy graph incurring low overheads and producing mostly precise results. The second phase uses these mostly precise results to bootstrap query evaluation on the larger original graph producing fully precise results. The effectiveness of this approach depends upon the quality of the proxy graph. Prior methods find proxy graphs that are either large or produce highly imprecise results.
We present a new form of proxy graph named the Core Graph (CG) that is not only small, it also produces highly precise results. A CG is a subgraph of the larger input graph that contains all vertices but on average contains only 10.7% of edges and yet produces precise results for 94.5-99.9% vertices in the graph for different queries. The finding of such an effective CG is based on our key new insight, namely, a small subset of non-zero centrality edges are responsible for determining the converged results of nearly all the vertices across different queries. We develop techniques to identify a CG that produces precise results for most vertices and optimizations to efficiently compute precise results of remaining vertices. Across six kinds of graph queries and four input graphs, CGs improved the performance of GPU-based Subway system by up to 4.48×, of out-of-core disk-based GridGraph system by up to 13.62×, and of Ligra in-memory graph processing system by up to 9.31×.</div>'

publication: '*EuroSys24: Proceedings of the Nineteenth European Conference on Computer Systems* <span style="color:red;">(Contributed Equally with the First Author)</span> <span style="color:green;"> (Acceptance Rate: 15.99%) </span>'
links:
- name: DOI
  url: https://dl.acm.org/doi/10.1145/3627703.3629571
- name: PDF
  url: "uploads/CoreGraph.pdf"
---

<style>
  .justify-text {
    text-align: justify;
  }
</style>