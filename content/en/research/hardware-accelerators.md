---
title: ""
date: 2025-11-12
slug: hardware-accelerators
share: false
commentable: false
editable: false
---

<div class="project-cards">
  <div class="project-card">
    <h3>Streaming Graph Accelerator — JetStream</h3>
    <p class="project-venue"><a href="/publication/jetstream-2021-micro/">MICRO 2021</a></p>
    <p>
      Streaming graphs, where nodes and edges change continuously, are central to modern workloads in social networks, bioinformatics, and large-scale data analytics. To accelerate these dynamic workloads, we developed JetStream, a hardware accelerator designed specifically for real-time graph updates. JetStream extends event-driven graph accelerator architectures to support edge insertions, deletions, and modifications while efficiently reusing prior computations to eliminate redundancy. By focusing computation only on the affected regions of the graph and optimizing memory access patterns, JetStream delivers significant performance improvements over conventional cold-start and software-based approaches, making it a powerful solution for high-throughput, evolving graphs.
    </p>
  </div>

  <div class="project-card">
    <h3>Evolving Graph Accelerator — MEGA</h3>
    <p class="project-venue"><a href="/publication/mega-2023-micro/">MICRO 2023</a></p>
    <p>
      Many modern applications — from social networks to bioinformatics — operate on evolving graphs that change continuously over time. Analyzing these graphs is difficult because queries must run across multiple snapshots to track how properties evolve. We developed MEGA, a hardware accelerator built specifically for efficient evolving-graph analytics. MEGA builds on the CommonGraph model to avoid costly deletions, supports event-driven edge updates, and executes multiple snapshots concurrently to maximize reuse. Its Batch-Oriented Execution (BOE) strategy schedules and pipelines updates for high locality and throughput. MEGA is the first accelerator to process multiple evolving-graph snapshots in parallel, delivering 24×–120× speedup over CommonGraph and 4.08×–5.98× over JetStream, the state-of-the-art streaming graph accelerator.
    </p>
  </div>

  <div class="project-card">
    <h3>Heterogeneous PIM for Graph Dynamic Programming — GEN-Graph</h3>
    <p class="project-venue"><a href="https://arxiv.org/abs/2604.15361">arXiv 2026</a></p>
    <p>
      Graph-based dynamic programming divides into two archetypes that stress different parts of a machine. Matrix-centric kernels such as all-pairs shortest path are dense and regular, and their limit is arithmetic throughput; topology-centric kernels such as sequence-to-graph alignment over pangenome references are sparse and pointer-chasing, and their limit is memory latency and effective bandwidth. No single homogeneous substrate serves both well, which is why programmable frameworks pay a penalty against task-specific ASICs and fixed-function designs cannot follow a new dataflow. GEN-Graph is a chiplet-based heterogeneous processing-in-memory accelerator that gives each archetype the substrate it wants: a PCM-based matrix tile performing bit-serial Floyd–Warshall and min-plus reductions in place, and an HBM3-based traversal tile whose near-memory processing elements run windowed bit-parallel alignment against banked SRAM. A tiered HBM–PCM–FeNAND hierarchy stages data by access frequency, and the hardware/software co-design — recursive partitioning sized to the memory arrays, reconfigurable bit-parallel logic, and compiler-driven mapping and scheduling — keeps every DP update exact rather than approximate while keeping both tiles busy.
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
.project-venue a,
.project-venue span {
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
.project-venue span {
  border-style: dashed;
  color: #777;
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
.dark .project-venue span {
  border-color: #4a4a4a;
  color: #a8a8a8;
}
.dark .project-venue a:hover,
.dark .project-venue a:focus {
  background: #4a8fd4;
  border-color: #4a8fd4;
  color: #fff;
}
</style>
