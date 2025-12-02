---
title: ""
date: 2025-11-12
slug: graph-analytics
share: false
commentable: false
editable: false
---

<div class="project-cards">
  <div class="project-card">
    <h3>Graph Analytics on Evolving Data — Common Graph</h3>
    <p>
      Evolving graphs change over time, requiring queries to run across many snapshots. Computing each snapshot independently wastes work, while traditional streaming approaches suffer from costly deletions and strict sequential updates. CommonGraph solves this by converting deletions into additions: it finds a shared base graph across all snapshots, computes the query once, and then incrementally adds the missing edges for each snapshot. This eliminates expensive mutations, enables reuse across snapshots, and removes sequential bottlenecks. Integrated with the KickStarter framework, CommonGraph provides a faster and more efficient way to analyze evolving graphs.
    </p>
  </div>

  <div class="project-card">
    <h3>Graph Analytics on Fixed Data — Core Graph</h3>
    <p>
      Iterative graph queries often incur high overhead because systems repeatedly move large graphs through the memory hierarchy and redundantly propagate values across edges. A common solution is to use a small proxy graph to approximate results before refining them on the full graph, but prior proxy graphs are either too large or too imprecise to be effective. We introduce the Core Graph (CG), a compact subgraph that retains all vertices but only a small fraction of edges while still producing highly accurate results. CGs work because only a small set of influential, high-centrality edges determine the final converged values for most vertices. By identifying these edges and refining only the few remaining vertices afterward, CGs provide a fast and accurate two-phase evaluation strategy that significantly accelerates iterative graph analytics.
    </p>
  </div>

  <div class="project-card">
    <h3>Redundancy Removal for Evolving Graphs - UVVs</h3>
    <p>
      Evaluating queries over large, irregular graphs is difficult, and the challenge grows when analyzing evolving graphs across many snapshots. Our study shows that in real workloads, most vertex-specific query results (e.g., SSSP distances) remain unchanged across the entire sequence of snapshots. We leverage these Unchanged Vertex Values (UVVs) by computing them once and limiting further work to only the vertices that truly change. To identify UVVs accurately, we introduce an intersection–union analysis that derives tight lower and upper bounds for each vertex across all snapshots; when the bounds match, the vertex is guaranteed to remain unchanged. For the remaining vertices, we perform concurrent incremental updates on all snapshots over a much smaller subgraph. Across several benchmarks, this dramatically reduces per-snapshot work and delivers significant speedups over state-of-the-art incremental graph analytics.
    </p>
  </div>

  <div class="project-card">
    <h3>Distributed Evovling Graph Analytics - Expressway</h3>
    <p>
      Distributed graph analytics often suffer from high communication overhead because large graphs must be processed across multiple machines using costly message passing. Expressway addresses this by identifying a small set of influential edges, called Highways, that heavily influence query results for their boundary vertices. By first running the query on these Highways alone, each machine can compute partial results locally without communication. These results are then used to initialize the full graph computation, allowing the algorithm to converge much faster. Integrated with existing distributed frameworks, Expressway significantly reduces communication overhead and speeds up both single-query and batched graph analytics.
    </p>
  </div>
</div>

<style>
.project-cards {
  display: flex;
  flex-direction: column;
  gap: 1.25rem;
  margin-top: 1.5rem;
}
.project-card {
  border: 1px solid #e0e0e0;
  border-radius: 10px;
  padding: 0.9rem 1.4rem;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
  background: #fff;
  width: 100%;
}
.project-card h3 {
  margin: 0 0 0.75rem 0;
}
.project-card p {
  margin: 0;
  text-align: justify;
}
</style>
