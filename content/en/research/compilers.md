---
title: "Compilers"
date: 2024-08-08
slug: compilers
share: false
commentable: false
editable: false
---

Explore the compiler projects highlighted below.

<div class="project-cards">
  <div class="project-card">
    <h3>Compiler Support for Hardware Accelerators</h3>
    <p>
      I extend MLIR-based infrastructures so domain scientists can map dynamic programming workloads
      directly onto custom accelerators. The pipeline captures DP recurrences, models data dependencies,
      and performs tiling, pipelining, and memory-placement optimizations before lowering to hardware-aware
      dialects. By automating these transformations, algorithm designers can rapidly evaluate FPGA/PIM
      implementations without writing RTL, accelerating hardware–software co-design.
    </p>
  </div>

  <div class="project-card">
    <h3>Binary Code Size Reduction</h3>
    <p>
      For embedded deployments I build compiler passes that shrink binary footprints through aggressive
      deduplication, layout-aware function merging, and data placement optimizations. The passes operate
      late in the toolchain to reason about actual machine instructions, enabling instruction reordering
      and constant pooling techniques that preserve performance while meeting tight memory budgets on
      microcontrollers and accelerator control processors.
    </p>
  </div>
</div>

<style>
.project-cards {
  display: grid;
  gap: 1.25rem;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  margin-top: 1.5rem;
}
.project-card {
  border: 1px solid #e0e0e0;
  border-radius: 10px;
  padding: 1.25rem;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
  background: #fff;
}
.project-card h3 {
  margin-top: 0;
  margin-bottom: 0.75rem;
}
.project-card p {
  margin: 0;
  text-align: justify;
}
</style>
