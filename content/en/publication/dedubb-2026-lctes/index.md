---
# Documentation: https://wowchemy.com/docs/managing-content/

title: ' DeduBB: Binary Code Size Reduction via Post-Link Basic Block De-duplication'
subtitle: ''
summary: ''
authors:
- Chaitanya Mamatha Ananda
- Mahbod Afarin
- Rajiv Gupta
- Sriraman Tallam
- Han Shen
- Xinliang David Li
tags: []
categories: []
date: '2026-06-17'
lastmod: 2026-06-17T19:57:59-04:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2026-06-17T23:57:59.485338Z'
publication_types:
- '1'
abstract: '<div class="justify-text"> Binary sizes of upgraded versions of software applications tend to be larger, primarily due to feature bloat. This poses various challenges, particularly for mobile applications. It affects upgrade rates directly impacting revenues, increases maintenance costs of supporting multiple versions, and prevents some users from getting critical security fixes. Code bloat also poses a problem for large warehouse-scale applications. Such applications experience performance degradation when their code size exceeds what smaller and more efficient code models can handle. In this paper, we introduce a post-link optimization technique called DeduBB, which deduplicates basic blocks of an application across procedure boundaries. As the prior techniques used function outlining to deduplicate identical code sequences, they missed out on many opportunities such as duplicate code patterns that manipulate the program stack. In addition, previous techniques were either limited to the scope of a module or lacked scalable implementations required to handle large warehouse-scale applications. Our technique, DeduBB, exploits inter-module opportunities and de-duplicates more code patterns than prior techniques as it uses a novel save-and-jump code sequence to execute deduplicated code blocks. In addition, DeduBB has been designed to work on scalable post-link optimizers and can even be applied to large warehouse-scale data center applications. Finally, DeduBB is profile-guided and can be applied selectively to infrequently executed cold basic blocks to not affect application performance. In fact, in several cases, the performance of the smaller application binary improves slightly due to reductions in its hot working set size. We have designed our technique for the state-of-the-art post-link optimizers, BOLT and Propeller. Experiments show that we can significantly reduce the code size of several benchmarks by 1.55% to 18.63%, on both Arm and x86 platforms, even on binaries that have already been heavily optimized for size using existing code size reduction features. For warehouse-scale binaries, DeduBB reduces code size by up to 25.8%. Finally, aided by profiles, our technique can retain over 82% of the maximal code size savings without affecting performance.</div>'
publication: '*LCTES 2026: Proceedings of the 27th ACM SIGPLAN/SIGBED International Conference on Languages, Compilers, and Tools for Embedded Systems*'
links:
- name: DOI
  url: https://dl.acm.org/doi/10.1145/3814943.3816169
---

<style>
  .justify-text {
    text-align: justify;
  }
</style>
