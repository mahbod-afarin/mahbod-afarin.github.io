---
# Documentation: https://wowchemy.com/docs/managing-content/

title: ' Expressway: Prioritizing Edges for Distributed Evaluation of Graph Queries'
subtitle: ''
summary: ''
authors:
- Abbas Mazloumi
- Mahbod Afarin
- Rajiv Gupta

tags: []
categories: []
date: '2023-12-158'
lastmod: 2023-12-18T19:57:59-04:00
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
publishDate: '2023-12-18T23:57:59.485338Z'
publication_types:
- '1'
abstract: '<div class="justify-text"> Distributed Graph analytics is being widely used in various domains for analyzing large real-world graphs. There have been numerous efforts to build distributed frameworks for graph analytics aimed at improving scalability. These frameworks enable the processing of huge graphs that do not fit in the memory of a single machine by imposing message-passing overhead among a cluster of multiple machines, underutilizing the available computing resources. To mitigate this, we present Expressway, a technique to identify important edges, i.e., Highways, that play a key role in delivering the results for their boundary vertices. Expressway first runs the queries using only Highways, reducing the number of edges that needed to be processed during the execution of a graph query significantly. Thus, it can be accomplished in each machine separately in the cluster, avoiding the message-passing overheads. Then Expressway takes the results from running the query on Highways and initializes the vertices to these values, enabling faster convergence of graph algorithms. Our experiments show applying Expressway on the state-of-the-art frameworks results in up to   speedup over the single-query framework and up to   speedup over the framework to run a batch of concurrent graph queries.</div>'
publication: '*2023 IEEE International Conference on Big Data (BigData)*'
links:
- name: DOI
  url: https://ieeexplore.ieee.org/document/10386860
- name: PDF
  url: uploads/expressway.pdf
---

<style>
  .justify-text {
    text-align: justify;
  }
</style>