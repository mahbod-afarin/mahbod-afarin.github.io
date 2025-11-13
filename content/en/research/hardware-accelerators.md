---
title: "Hardware Accelerators"
date: 2024-08-08
slug: hardware-accelerators
share: false
commentable: false
editable: false
---

### Streaming Graph Accelerator — JetStream

JetStream evaluates queries over streaming graphs where edges are constantly inserted, removed, or updated. By adopting an event-driven execution model, the accelerator limits computation to the affected neighborhood, reuses intermediate state, and reorganizes memory access patterns for higher bandwidth utilization. JetStream reduces cold-start recomputation by up to 90% and achieves 18× speedups over optimized CPU frameworks at comparable batch sizes.

### Evolving Graph Accelerator — MEGA

MEGA targets evolving graphs that require evaluating a query across a sequence of snapshots. It builds on the CommonGraph software model and introduces Batch-Oriented Execution so snapshots can be processed concurrently. Combined with incremental event streaming and tailored memory hierarchies, MEGA sustains high throughput while avoiding the overhead of handling deletions explicitly.

### Design Principles

- Event-driven scheduling that matches graph update semantics.
- Custom data paths and scratchpad hierarchies to maximize locality.
- Hardware–software co-design that surfaces accelerator capabilities through compiler support and APIs.
