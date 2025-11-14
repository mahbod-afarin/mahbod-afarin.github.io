---
title: "Hardware Accelerators"
date: 2025-11-13
slug: hardware-accelerators
share: false
commentable: false
editable: false
---

<div class="project-cards">
  <div class="project-card">
    <h3>Streaming Graph Accelerator — JetStream</h3>
    <p>
      JetStream evaluates queries over rapidly changing graphs where edges are constantly inserted,
      removed, or updated. An event-driven execution model limits computation to the affected
      neighborhood, reuses intermediate state, and reshapes memory access for higher bandwidth.
      The design trims cold-start recomputation by up to 90% and delivers 18× speedups over optimized
      CPU frameworks at comparable batch sizes.
    </p>
  </div>

  <div class="project-card">
    <h3>Evolving Graph Accelerator — MEGA</h3>
    <p>
      MEGA targets evolving graphs that require evaluating queries across snapshots. Built on the
      CommonGraph software model, it introduces Batch-Oriented Execution so snapshots can be processed
      concurrently while incremental event streaming feeds updates efficiently. Custom memory hierarchies
      keep throughput high and avoid the overhead of explicitly handling deletions.
    </p>
  </div>

  <div class="project-card">
    <h3>Design Principles</h3>
    <p>
      Across both accelerators I rely on event-driven scheduling tuned to graph semantics, bespoke scratchpad
      hierarchies that maximize locality, and hardware–software co-design so compiler toolchains expose the
      accelerator capabilities through approachable APIs.
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
