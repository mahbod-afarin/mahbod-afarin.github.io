---
title: ""
date: 2025-11-12
slug: compilers
share: false
commentable: false
editable: false
---

<div class="project-cards">
  <div class="project-card">
    <h3>Compiler Support for Hardware Accelerators</h3>
    <p>
      Bioinformatics and graph dynamic-programming algorithms are slow and difficult to program due to their complex data dependencies. While recent work has introduced unified compilers for hyperdimensional-computing accelerators, there is still no analogous compiler support for dynamic-programming hardware accelerators, leaving developers dependent on manual, hardware-specific tuning. To address this gap, we developed a unified MLIR-based compiler that targets three different DP hardware accelerators. Our compiler automatically transforms high-level algorithms into highly optimized hardware instructions, eliminating manual tuning and making DP accelerators far easier to program and deploy.
    </p>
  </div>

  <div class="project-card">
    <h3>Binary Code Size Reduction</h3>
    <p>
      Modern software binaries keep growing due to feature expansion, causing slow upgrades, higher maintenance costs, and performance issues in both mobile and large-scale applications. To combat code bloat, we developed DeduBB, a post-link optimizer that de-duplicates identical basic blocks across functions and modules. Unlike earlier methods, it detects a wider range of redundant code patterns and replaces them with a lightweight save-and-jump sequence. Designed for scalability, DeduBB integrates with state-of-the-art post-link optimizers and uses profiling to safely reduce code size without harming performance.
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
  margin-top: 0;
  margin-bottom: 0.75rem;
}
.project-card p {
  margin: 0;
  text-align: justify;
}
</style>
