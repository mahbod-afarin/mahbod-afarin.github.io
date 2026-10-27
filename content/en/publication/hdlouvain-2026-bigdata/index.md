---
# Documentation: https://wowchemy.com/docs/managing-content/

title: ' HDLouvain: High-Throughput Incremental Clustering for Hyperdimensional Data'
subtitle: ''
summary: ''
authors:
- Beenish Gul
- Mahbod Afarin
- Farhat Ahmed
- Sumukh Pinge
- Tsung-Han Lu
- Tajana Rosing
- Kevin Skadron
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
abstract: '<div class="justify-text"> Modern shotgun proteomics generates tens of thousands of tandem mass spectra per hour, producing hundreds of gigabytes of data that strain conventional clustering pipelines. DBSCAN and hierarchical agglomerative clustering (HAC) offer flexible similarity search, but DBSCAN is unstable across varying data densities, HAC costs O(n²), and both yield poor cluster quality. Graph-based methods such as Louvain produce high-quality clusters but scale poorly on streaming data. We observe that Louvain''s poor scalability can be resolved without sacrificing its quality, and present HDLouvain, which combines Louvain community detection with the bit-parallel similarity computation of hyperdimensional computing (HDC). HDLouvain partitions a bootstrap fraction of the stream into precursor-mass buckets, applies Louvain to each bucket''s kNN similarity graph, and condenses each community into a single binary hypervector by bitwise-majority bundling rather than iterative centroid recomputation. New spectra are assigned by a GPU-accelerated Hamming distance lookup against representatives in their mass bucket, or seed a new cluster when no match meets a similarity threshold τ, so the partition grows incrementally without full re-clustering. On five PRIDE datasets (0.99M to 21.13M spectra), sweeping the bootstrap fraction α from 0.2 to 0.9 exposes an explicit, monotonic throughput-fidelity trade-off. On PXD003258, speedup ranges from 4.5× at α=0.3 to 1.65× at α=0.7. Modularity rises from 0.75-0.76 at α=0.2 to 0.95-0.97 at α=0.9, never more than 8% below full static recomputation. The Louvain stage achieves 0.86-0.93 normalized mutual information (NMI) on LFR benchmark networks with 30k to 2M nodes, whereas DBSCAN and HAC degrade to 0.57.</div>'
publication: '*2026 IEEE International Conference on Big Data (BigData)* <span style="color:green;"> (Acceptance Rate: 19.4%) </span>'
links:
- name: arXiv
  url: https://arxiv.org/abs/2610.30687
---

<style>
  .justify-text {
    text-align: justify;
  }
</style>
