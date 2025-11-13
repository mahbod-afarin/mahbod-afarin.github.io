+++
date = "2024-08-08T00:00:00"
+++

<div style="text-align: justify;">

### Research

</div>

<div class="research-tabs">
  <div class="research-tab-buttons">
    <button class="research-tab-button active" data-target="tab-compilers">Compilers</button>
    <button class="research-tab-button" data-target="tab-accelerators">Hardware Accelerators</button>
    <button class="research-tab-button" data-target="tab-graphs">Graph Analytics</button>
  </div>

  <div id="tab-compilers" class="research-tab-content active" style="text-align: justify;">
    <h4>Compiler Support for Specialized Hardware</h4>
    <p>
      I extend MLIR-based compiler infrastructures so that domain experts can target
      dynamic programming accelerators without writing low-level hardware descriptions.
      The compiler pipeline captures DP recurrences, applies tiling, pipelining, and memory-placement
      optimizations, and emits hardware-aware instructions for FPGA- and PIM-based fabrics.
      This automation closes the gap between algorithm designers and accelerator hardware,
      delivering substantial performance-per-watt improvements with reusable transformation passes.
    </p>
  </div>

  <div id="tab-accelerators" class="research-tab-content" style="text-align: justify;">
    <h4>Hardware Accelerators</h4>
    <p>
      I co-design streaming and evolving graph accelerators that keep pace with highly dynamic datasets.
      JetStream reduces streaming graph query time by reusing intermediate results and reshaping memory
      access to sustain high bandwidth, while MEGA executes batched snapshots concurrently to evaluate
      evolving graphs efficiently. These designs show how event-driven scheduling, custom data paths,
      and domain-specific memory hierarchies unlock order-of-magnitude speedups over CPU/GPU baselines.
    </p>
  </div>

  <div id="tab-graphs" class="research-tab-content" style="text-align: justify;">
    <h4>Graph Analytics & Algorithms</h4>
    <p>
      My algorithmic work focuses on exposing parallelism and reducing redundancy in graph workloads.
      I design techniques that stabilize vertex values, compress traversal work, and balance computation
      across heterogeneous hardware targets. By combining compiler-driven optimizations with new graph
      formulations, my frameworks scale to billion-edge graphs while maintaining accuracy, resilience,
      and predictable execution time across CPUs, GPUs, and bespoke accelerators.
    </p>
  </div>
</div>

<style>
.research-tabs {
  margin-top: 1.5rem;
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  padding: 0.5rem;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}
.research-tab-buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin-bottom: 0.5rem;
}
.research-tab-button {
  flex: 1 1 150px;
  padding: 0.5rem 0.75rem;
  border: 1px solid #4CAF50;
  border-radius: 4px;
  background: #fff;
  cursor: pointer;
  font-weight: 600;
  color: #2b2b2b;
  transition: background 0.2s ease, color 0.2s ease;
}
.research-tab-button.active {
  background: #4CAF50;
  color: #fff;
}
.research-tab-content {
  display: none;
  padding: 0.5rem;
}
.research-tab-content.active {
  display: block;
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function () {
  const buttons = document.querySelectorAll('.research-tab-button');
  const sections = document.querySelectorAll('.research-tab-content');

  buttons.forEach((button) => {
    button.addEventListener('click', () => {
      buttons.forEach((btn) => btn.classList.remove('active'));
      sections.forEach((section) => section.classList.remove('active'));

      button.classList.add('active');
      const target = document.getElementById(button.dataset.target);
      if (target) {
        target.classList.add('active');
      }
    });
  });
});
</script>
