+++
date = "2024-08-08T00:00:00"
+++

<div style="text-align: justify;">

### Research

</div>

<p style="text-align: justify;">
Explore the three core areas of my research by selecting a focus below. Each circle highlights a
different pillar and links to a dedicated page with deeper dives, publications, and current projects.
</p>

<div class="research-circles">
  <a class="research-circle" href="/research/compilers/">
    <div class="circle-image" style="background-image: url('/uploads/research-compilers.png');" aria-hidden="true"></div>
    <div class="circle-label">Compiler Optimization</div>
  </a>

  <a class="research-circle" href="/research/hardware-accelerators/">
    <div class="circle-image" style="background-image: url('/uploads/research-hardware.png');" aria-hidden="true"></div>
    <div class="circle-label">Hardware Accelerators</div>
  </a>

  <a class="research-circle" href="/research/graph-analytics/">
    <div class="circle-image" style="background-image: url('/uploads/research-graph.png');" aria-hidden="true"></div>
    <div class="circle-label">Graph Analytics</div>
  </a>
</div>

<style>
.research-circles {
  display: flex;
  flex-wrap: wrap;
  gap: 1.5rem;
  justify-content: center;
  margin-top: 1.5rem;
}
.research-circle {
  flex: 1 1 200px;
  max-width: 240px;
  text-align: center;
  text-decoration: none;
  color: inherit;
}
.circle-image {
  width: 220px;
  height: 220px;
  margin: 0 auto;
  border-radius: 50%;
  background-size: cover;
  background-position: center;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.2);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.research-circle:hover .circle-image,
.research-circle:focus .circle-image {
  transform: translateY(-6px);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.25);
}
.circle-label {
  margin-top: 0.75rem;
  font-size: 1.1rem;
  font-weight: 600;
}
@media (max-width: 600px) {
  .circle-image {
    width: 180px;
    height: 180px;
  }
}
</style>
