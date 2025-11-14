---
title: "Hardware Accelerators"
date: 2025-11-12
slug: hardware-accelerators
share: false
commentable: false
editable: false
---

<div class="project-cards">
  <div class="project-card">
    <h3>Streaming Graph Accelerator — JetStream</h3>
    <p>
      Streaming graphs, where nodes and edges change continuously, are central to modern workloads in social networks, bioinformatics, and large-scale data analytics. To accelerate these dynamic workloads, we developed JetStream, a hardware accelerator designed for real-time graph updates. JetStream extends event-driven graph accelerator architectures to support edge insertions, deletions, and modifications while reusing prior computations to eliminate redundancy. By focusing computation only on the affected regions of the graph and optimizing memory access patterns, JetStream delivers significant performance improvements over conventional cold-start and software-based approaches, making it a powerful solution for high-throughput, evolving graph analytics.
    </p>
  </div>

  <div class="project-card">
    <h3>Evolving Graph Accelerator — MEGA</h3>
    <p>
      Many modern applications—from social networks to bioinformatics—operate on evolving graphs that change continuously over time. Analyzing these graphs is difficult because queries must run across multiple snapshots to track how properties evolve. We developed MEGA, a hardware accelerator built specifically for efficient evolving-graph analytics. MEGA builds on the CommonGraph model to avoid costly deletions, supports event-driven edge updates, and executes multiple snapshots concurrently to maximize reuse. Its Batch-Oriented Execution (BOE) strategy schedules and pipelines updates for high locality and throughput. MEGA is the first accelerator to process multiple evolving-graph snapshots in parallel, delivering significant speedups over both software frameworks and prior streaming graph accelerators.
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
