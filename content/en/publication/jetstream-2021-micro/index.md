---
# Documentation: https://wowchemy.com/docs/managing-content/

title: ' JetStream: Graph Analytics on Streaming Data with Event-Driven Hardware Accelerator'
subtitle: ''
summary: ''
authors:
- Shafiur Rahman
- Mahbod Afarin
- Nael Abu-Ghazaleh
- Rajiv Gupta
tags: []
categories: []
date: '2021-10-17'
lastmod: 2021-10-18T19:57:59-04:00
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
publishDate: '2021-10-18T23:57:59.485338Z'
publication_types:
- '1'
abstract: '<div class="justify-text"> Graph Processing is at the core of many critical emerging workloads operating on unstructured data, including social network analysis, bioinformatics, and many others. Many applications operate on graphs that are constantly changing, i.e., new nodes and edges are added or removed over time. In this paper, we present JetStream, a hardware accelerator for evaluating queries over streaming graphs and capable of handling additions, deletions, and updates of edges. JetStream extends a recently proposed event-based accelerator for graph workloads to support streaming updates. It handles both accumulative and monotonic graph algorithms via an event-driven computation model that limits accesses to a smaller subset of the graph vertices, efficiently reuses the prior query results to eliminate redundancy, and optimizes the memory access pattern for enhanced memory bandwidth utilization. To the best of our knowledge, JetStream is the first graph accelerator that supports streaming graphs, reducing the computation time by 90% compared with cold-start computation using an existing accelerator. In addition, JetStream achieves about 18 × speedup over KickStarter and GraphBolt software frameworks at the large baseline batch sizes that these systems use with significantly higher speedup at smaller batch sizes.</div>'
publication: '*MICRO21: 54th Annual IEEE/ACM International Symposium on Microarchitecture* <span style="color:green;"> (Acceptance Rate: 21.74%) </span>'
links:
- name: DOI
  url: https://dl.acm.org/doi/10.1145/3466752.3480126
- name: PDF
  url: uploads/jetstream.pdf
---

<style>
  .justify-text {
    text-align: justify;
  }
</style>