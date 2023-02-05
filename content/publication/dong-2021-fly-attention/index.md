---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'On-the-Fly Attention Modulation for Neural Generation'
subtitle: ''
summary: ''
authors:
- Yue Dong
- Chandra Bhagavatula
- Ximing Lu
- Jena D. Hwang
- Antoine Bosselut
- Jackie Chi Kit Cheung
- Yejin Choi
tags: []
categories: []
date: '2021-08-01'
lastmod: 2022-07-18T19:57:59-04:00
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
publishDate: '2022-07-18T23:57:59.485338Z'
publication_types:
- '1'
abstract: 'Despite considerable advancements with deep neural language models (LMs), neural text generation still suffers from degeneration: the generated text is repetitive, generic, self-contradictory, and often lacks commonsense. Our analyses on sentence-level attention patterns in LMs reveal that neural degeneration may be associated with insufficient learning of task-specific characteristics by the attention mechanism. This finding motivates on-the-fly attention modulation – a simple but effective method that enables the injection of priors into attention computation during inference. Automatic and human evaluation results on three text generation benchmarks demonstrate that attention modulation helps LMs generate text with enhanced fluency, creativity, and commonsense reasoning, in addition to significantly reduce sentence-level repetition.'
publication: '*Findings of the Association for Computational Linguistics (Findings of ACL)*'
links:
- name: Arxiv
  url: https://arxiv.org/pdf/2101.00371.pdf
- name: ACL Anthology
  url: https://aclanthology.org/2021.findings-acl.107/
---
