---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'MEGA Evolving Graph Accelerator'
subtitle: ''
summary: ''
authors:
- Chao Gao
- Mahbod Afarin
- Shafiur Rahman
- Nael Abu-Ghazaleh
- Rajiv Gupta
tags: []
categories: []
date: '2023-12-08'
lastmod: 2023-08-18T19:57:59-04:00
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
publishDate: '2023-08-18T23:57:59.485338Z'
publication_types:
- '1'
abstract: '<div class="justify-text"> Graph Processing is an emerging workload for applications working with unstructured data, such as social network analysis, transportation networks, bioinformatics and operations research. We examine the problem of graph analytics over evolving graphs, which are graphs that change over time. The problem is challenging because it requires evaluation of a graph query on a sequence of graph snapshots over a time window, typically to track the progression of a property over time. In this paper, we introduce MEGA, a hardware accelerator designed for efficiently evaluating queries over evolving graphs. MEGA leverages CommonGraph, a recently proposed software approach for incrementally processing evolving graphs that gains efficiency by avoiding the need to process expensive deletions by converting them into additions. MEGA supports incremental event-based streaming of edge additions as well as execution of multiple snapshots concurrently to support evolving graphs. We propose Batch-Oriented-Execution (BOE), a novel batch-update scheduling technique that activates snapshots that share batches simultaneously to achieve both computation and data reuse. We introduce optimizations that pack compatible batches together, and pipeline batch processing. To the best of our knowledge, MEGA is the first graph accelerator for evolving graphs that evaluates graph queries over multiple snapshots simultaneously. MEGA achieves 24 × -120 × speedup over CommonGraph. It also achieves speedups ranging from 4.08 × to 5.98 × over JetStream, a state-of-the-art streaming graph accelerator.</div>'
publication: '*MICRO23: Proceedings of the 56th Annual IEEE/ACM International Symposium on Microarchitecture* <span style="color:red;">(Contributed Equally with the First Author)</span> <span style="color:green;"> (Acceptance Rate: 22%) </span>'
links:
- name: DOI
  url: https://dl.acm.org/doi/10.1145/3613424.3614260
- name: PDF
  url: uploads/mega.pdf
---


<style>
  .justify-text {
    text-align: justify;
  }
</style>