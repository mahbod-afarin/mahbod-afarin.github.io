---
# Documentation: https://wowchemy.com/docs/managing-content/

title: ' GenMLIR: An MLIR Compiler for Dynamic Programming Workloads on Tier-Aware 3D-DRAM PIM'
subtitle: ''
summary: ''
authors:
- Mahbod Afarin
- Tsung-Han Lu
- Tajana Rosing
tags: []
categories: []
date: '2026-09-10'
lastmod: 2026-09-10T19:57:59-04:00
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
publishDate: '2026-09-10T23:57:59.485338Z'
publication_types:
- '1'
abstract: '<div class="justify-text"> Processing-in-Memory (PIM) on monolithic 3D (M3D) DRAM is a promising answer to the memory wall for data-intensive dynamic programming (DP), yet extracting its performance today demands hand-written kernels: the programmer must pick a tile size, place data across non-uniform-latency memory tiers, partition work between heterogeneous processing units, and insert the right broadcasts and queues by hand. We present GenMLIR, an MLIR compiler that automates this mapping for tier-aware 3D PIM. GenMLIR encodes the semi-ring generalized grid update, the algebraic form shared by all-pairs shortest path (APSP) and sequence alignment, as a first-class IR abstraction, and lowers it through four GenDRAM-aware pass groups that derive blocked tiling, tier-aware placement, tile-to-PU assignment, and explicit communication. We also characterize precisely which DP recurrences the abstraction admits and which it does not. On the GenDRAM architecture, GenMLIR-generated code runs up to 5.8× (APSP) and 16.7× (alignment) faster than a lowering without compiler support, and 1.2-1.4× faster than a standard affine-tiling PIM compiler we also implement, reaching 90-100% of an achievable-performance bound. It expresses these workloads in 4-9 lines instead of 300-500 and compiles in a negligible fraction of runtime.</div>'
publication: '*ASP-DAC 2027: Proceedings of the 32nd Asia and South Pacific Design Automation Conference*'
links:
- name: arXiv
  url: https://arxiv.org/abs/2610.09156
---

<style>
  .justify-text {
    text-align: justify;
  }
</style>
