---
# Documentation: https://wowchemy.com/docs/managing-content/

title: ' Indexing Evolving Graphs via Query Evolution Prediction'
subtitle: ''
summary: ''
authors:
- Chao Gao
- Xizhe Yin
- Mahbod Afarin
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
abstract: '<div class="justify-text"> Real-world graphs evolve, and analytical tasks over them are posed across a sequence of temporally indexed snapshots. A recurring question is not what a query returns on one snapshot but when its result changes across many. Answering it directly requires evaluating the query on every snapshot, and most of that work is wasted. Across six evolving graphs, 22% to 94% of one-to-all evaluations reproduce the preceding snapshot''s result exactly. We present EvoGIndex, an index that locates the time windows in which a query result changes without evaluating the query on every snapshot. Distance bounds have been used in evolving-graph systems to make an already-issued query converge faster. EvoGIndex uses them to decide whether the query needs to be issued at all, turning a query optimization into a temporal index. A core graph skeleton is built once from a small set of base vertices and projected onto each snapshot in linear time without evaluating queries, and a generalized triangle inequality over it yields a bound interval per snapshot whose movement between consecutive snapshots is the change signal. We state the query class the bound covers, monotonic vertex-centric iterative queries over a totally ordered domain with invertible path composition, and which queries fall outside it. Across six graphs, seven benchmarks and six time windows EvoGIndex retains 22% of the edges, recovers 84–88% of changed vertices, raises precision from 54% to 95% as the window widens, and delivers up to 240× speedup over RisGraph by eliminating wasteful computations. We also report where it fails. For reachability the value domain is Boolean, the interval cannot narrow, and prediction loses to a no-change baseline on four of the six graphs.</div>'
publication: '*2026 IEEE International Conference on Big Data (BigData)* <span style="color:green;"> (Acceptance Rate: 19.4%) </span>'
links: []
---

<style>
  .justify-text {
    text-align: justify;
  }
</style>
