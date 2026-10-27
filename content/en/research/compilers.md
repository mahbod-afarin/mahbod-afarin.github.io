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
    <h3>Compiling Dynamic Programming for Processing-in-Memory — GenMLIR</h3>
    <p class="project-venue"><a href="/publication/genmlir-2027-aspdac/">ASP-DAC 2027</a></p>
    <p>
      Dynamic-programming (DP) workloads such as all-pairs shortest path and sequence alignment are a natural fit for processing-in-memory (PIM) on monolithic 3D DRAM, but extracting that performance today means writing kernels by hand: picking tile sizes, placing data across non-uniform-latency memory tiers, partitioning work among heterogeneous processing units, and inserting the right broadcasts and queues manually. GenMLIR is an MLIR compiler that automates this mapping. It encodes the semi-ring generalized grid update — the algebraic form shared by all-pairs shortest path and sequence alignment — as a first-class IR abstraction, then lowers it through hardware-aware pass groups that derive blocked tiling, tier-aware placement, tile-to-PU assignment, and explicit communication. The generated code runs up to 5.8× (APSP) and 16.7× (alignment) faster than a lowering without compiler support and 1.2–1.4× faster than standard affine tiling, while expressing each workload in 4–9 lines instead of several hundred.
    </p>
  </div>

  <div class="project-card">
    <h3>Approximation Tuning for Hyperdimensional Computing — ApproxHDC</h3>
    <p class="project-venue"><a href="/publication/approxhdc-2027-asplos/">ASPLOS 2027</a></p>
    <p>
      Hyperdimensional computing (HDC) is intrinsically tolerant to noise and approximation, which makes it a strong match for heterogeneous hardware — CPUs, GPUs, and FPGAs, as well as in-memory technologies such as ReRAM and phase-change memory. Deciding <em>which</em> approximations to apply and how aggressively, however, is a search problem whose space grows exponentially with the number of operations. ApproxHDC extends the HPVM-HDC compiler infrastructure to automatically identify the approximation opportunities in an HDC application, construct the design space spanning both software and hardware levels, and search it efficiently under a user-specified quality-of-service constraint, retargeting the result across CPU, GPU, and simulated ReRAM/PCM backends. It reaches up to 17.25× speedup on CPUs, 15.02× on GPUs, and 4.69× on SpecPCM, outperforming the prior state-of-the-art MicroHD by 3.49× at the same accuracy bar.
    </p>
  </div>

  <div class="project-card">
    <h3>Binary Code Size Reduction — DeduBB</h3>
    <p class="project-venue"><a href="/publication/dedubb-2026-lctes/">LCTES 2026</a></p>
    <p>
      Modern software binaries keep growing due to feature expansion, which slows upgrades, raises maintenance costs, and degrades performance once code size outgrows the smaller, more efficient code models. DeduBB is a post-link optimizer that de-duplicates identical basic blocks across procedure and module boundaries. Where earlier techniques relied on function outlining and therefore missed many duplicates — including code patterns that manipulate the program stack — DeduBB replaces redundant blocks with a lightweight save-and-jump sequence that covers far more cases. Built for the scalable post-link optimizers BOLT and Propeller, and guided by profiles so that only cold blocks are touched, it shrinks benchmark binaries by 1.55%–18.63% on Arm and x86 and warehouse-scale binaries by up to 25.8%, retaining over 82% of the maximal savings without hurting performance. The work was done during my student researcher position on the Compiler Optimization team at Google.
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
