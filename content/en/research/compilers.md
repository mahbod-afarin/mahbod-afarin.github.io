---
title: "Compilers"
date: 2024-08-08
slug: compilers
share: false
commentable: false
editable: false
---

### Compiler Support for Specialized Hardware

I extend MLIR-based compiler infrastructures so that domain scientists can map dynamic programming (DP) algorithms onto custom accelerators without writing RTL or low-level intrinsics. The pipeline captures DP recurrences, models their data dependencies, and applies tiling, pipelining, and memory-placement optimizations before lowering to hardware-aware dialects. This automation closes the gap between high-level algorithm design and FPGA/PIM implementations, enabling rapid exploration of hardware–software co-design spaces.

### Domain-Specific Optimization Passes

My compiler passes reuse abstractions across DP kernels, exposing opportunities for loop fusion, iteration space pruning, and systolic scheduling. Because the transformations are implemented in MLIR, I can compose them with existing affine and vector optimizations, making the toolchain extensible and reusable for new accelerators.

### Outcomes

- Automated generation of accelerator-ready kernels from mathematical DP descriptions.
- Significant performance-per-watt improvements versus hand-written baselines.
- Modular passes that downstream research teams can adopt for their own domains.
