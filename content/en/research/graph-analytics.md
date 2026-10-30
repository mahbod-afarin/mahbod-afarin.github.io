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
    <h3>Graph Analytics on Evolving Data — CommonGraph</h3>
    <p class="project-venue"><a href="/publication/commongraph-2023-asplos/">ASPLOS 2023</a><a href="/publication/commongraph-2023-hopc/">HOPC 2023</a></p>
    <p>
      Evolving graphs change over time, requiring queries to run across many snapshots. Computing each snapshot independently wastes work, while traditional streaming approaches suffer from costly deletions and strict sequential updates. CommonGraph solves this by converting deletions into additions: it finds a shared base graph across all snapshots, computes the query once, and then incrementally adds the missing edges for each snapshot. This eliminates expensive mutations, enables reuse across snapshots, and removes sequential bottlenecks. Integrated with the KickStarter framework, CommonGraph provides a faster and more efficient way to analyze evolving graphs, improving performance by 1.38×–8.17× across multiple benchmarks.
    </p>
  </div>

  <div class="project-card">
    <h3>Redundancy Removal for Evolving Graphs — UVVs</h3>
    <p class="project-venue"><a href="/publication/uvv-2025-arxiv/">IPDPS 2026</a></p>
    <p>
      Evaluating queries over large, irregular graphs is difficult, and the challenge grows when analyzing evolving graphs across many snapshots. Our study shows that in real workloads, most vertex-specific query results (e.g., SSSP distances) remain unchanged across the entire sequence of snapshots. We leverage these Unchanged Vertex Values (UVVs) by computing them once and limiting further work to only the vertices that truly change. To identify UVVs accurately, we introduce an intersection–union analysis that derives tight lower and upper bounds for each vertex across all snapshots; when the bounds match, the vertex is guaranteed to remain unchanged. For the remaining vertices, we perform concurrent incremental updates on all snapshots over a much smaller subgraph. Across several benchmarks this cuts per-snapshot work to under 42% of the vertices on under 32% of the edges, delivering 2.01×–12.23× speedups over the state-of-the-art incremental baseline.
    </p>
  </div>

  <div class="project-card">
    <h3>Temporally Consistent Graph Sampling — Sagas</h3>
    <p class="project-venue"><a href="/publication/sagas-2026-bigdata/">IEEE BigData 2026</a></p>
    <p>
      Sampling is the standard way to make a large graph tractable for visualization, approximate analytics, and GNN training, but on an evolving graph a sample drawn independently per snapshot destroys the very thing the analysis is after: consecutive samples differ because of sampling randomness rather than because the graph changed, so a trend read off the sample need not hold on the original. Sagas is the first temporally consistent sampling system for evolving graphs. It draws a sample on one primary snapshot and projects it forward and backward in time, repairing any edge missing from a target snapshot with an alternate path, so that both snapshot consistency and the graph's evolutionary trends survive the projection. The work also defines the metrics that make temporal consistency measurable: structural similarity, which asks whether changes between consecutive samples track changes in the original graph, and trend divergence, which asks whether a property moves in the same direction on both. Because repair dominates the cost, Sagas consolidates repairs that share a source vertex into a single parallel traversal and runs them over a compact graph skeleton, together improving performance by nearly four orders of magnitude over sequential repair and improving temporal consistency by up to 99.1%.
    </p>
  </div>

  <div class="project-card">
    <h3>Temporal Indexing for Evolving Graphs — EvoGIndex</h3>
    <p class="project-venue"><a href="/publication/indexing-2026-bigdata/">IEEE BigData 2026</a></p>
    <p>
      When the same query is issued across a sequence of snapshots, most of those evaluations are wasted: across six evolving graphs, 22% to 94% of one-to-all evaluations reproduce the preceding snapshot's result exactly. EvoGIndex locates the time windows in which a result actually changes, without evaluating the query on every snapshot. Distance bounds already exist in evolving-graph systems, where they make an already-issued query converge faster; EvoGIndex instead uses them to decide whether the query needs to be issued at all, turning a query optimization into a temporal index. A core graph skeleton is built once from a small set of base vertices and projected onto each snapshot in linear time with no query evaluation, and a generalized triangle inequality over it yields a bound interval per snapshot whose movement between consecutive snapshots is the change signal. The paper states the query class the bound is sound for — monotonic vertex-centric iterative queries over a totally ordered domain with invertible path composition — and reports where it fails: for reachability the value domain is Boolean, the interval cannot narrow, and prediction loses to a trivial no-change baseline. Within that scope it recovers 84–88% of changed vertices at a precision rising to 95%, and delivers up to 240× speedup over RisGraph.
    </p>
  </div>

  <div class="project-card">
    <h3>Graph Analytics on Fixed Data — Core Graph</h3>
    <p class="project-venue"><a href="/publication/coregraph-2024-eurosys/">EuroSys 2024</a></p>
    <p>
      Iterative graph queries often incur high overhead because systems repeatedly move large graphs through the memory hierarchy and redundantly propagate values across edges. A common solution is to use a small proxy graph to approximate results before refining them on the full graph, but prior proxy graphs are either too large or too imprecise to be effective. We introduce the Core Graph (CG), a compact subgraph that retains all vertices but only a small fraction of edges while still producing highly accurate results. CGs work because only a small set of influential, high-centrality edges determine the final converged values for most vertices. By identifying these edges and refining only the few remaining vertices afterward, CGs provide a fast and accurate two-phase evaluation strategy that significantly accelerates iterative graph analytics.
    </p>
  </div>

  <div class="project-card">
    <h3>Distributed Graph Query Evaluation — Expressway</h3>
    <p class="project-venue"><a href="/publication/expressway-2023-bigdata/">IEEE BigData 2023</a></p>
    <p>
      Distributed graph analytics often suffer from high communication overhead because large graphs must be processed across multiple machines using costly message passing. Expressway addresses this by identifying a small set of influential edges, called Highways, that heavily influence query results for their boundary vertices. By first running the query on these Highways alone, each machine can compute partial results locally without communication. These results are then used to initialize the full graph computation, allowing the algorithm to converge much faster. Integrated with existing distributed frameworks, Expressway significantly reduces communication overhead and speeds up both single-query and batched graph analytics.
    </p>
  </div>

  <div class="project-card">
    <h3>Scalable Graph-Based Clustering — HDLouvain</h3>
    <p class="project-venue"><a href="/publication/hdlouvain-2026-bigdata/">IEEE BigData 2026</a></p>
    <p>
      Modern shotgun proteomics produces tens of thousands of tandem mass spectra per hour, far beyond what conventional clustering pipelines handle gracefully: DBSCAN is unstable across varying densities, hierarchical agglomerative clustering costs O(n²), and graph-based Louvain community detection gives the best cluster quality but scales poorly on streaming data. HDLouvain shows those two properties are not fundamentally at odds. It runs Louvain over per-bucket k-NN similarity graphs built from a bootstrap fraction of the stream, condenses each community into a single binary hypervector through bitwise-majority bundling instead of iterative centroid recomputation, and assigns new spectra by GPU-accelerated Hamming-distance lookup — so the partition grows incrementally without re-clustering everything. On PRIDE datasets of 0.99M–21.13M spectra this exposes an explicit throughput–fidelity trade-off, reaching 4.5× speedup while staying within 8% of the modularity of full static recomputation.
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
  margin: 0 0 0.5rem 0;
}
.project-card p {
  margin: 0;
  text-align: justify;
}
.project-venue {
  margin: 0 0 0.75rem 0 !important;
  text-align: left !important;
}
.project-venue a {
  display: inline-block;
  margin: 0 0.35rem 0.35rem 0;
  padding: 0.12rem 0.65rem;
  font-size: 0.78rem;
  font-weight: 600;
  letter-spacing: 0.02em;
  border: 1px solid #d5d5d5;
  border-radius: 999px;
  color: #555;
  text-decoration: none;
  transition: background 0.2s ease, color 0.2s ease, border-color 0.2s ease;
}
.project-venue a:hover,
.project-venue a:focus {
  background: #2e74b5;
  border-color: #2e74b5;
  color: #fff;
}
.dark .project-card {
  background: #1e1e1e;
  border-color: #3a3a3a;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.4);
}
.dark .project-card h3,
.dark .project-card p {
  color: #f5f5f5;
}
.dark .project-venue a {
  border-color: #4a4a4a;
  color: #cfcfcf;
}
.dark .project-venue a:hover,
.dark .project-venue a:focus {
  background: #4a8fd4;
  border-color: #4a8fd4;
  color: #fff;
}
</style>
