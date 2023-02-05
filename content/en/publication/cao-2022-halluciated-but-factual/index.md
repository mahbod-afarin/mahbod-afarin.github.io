---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Hallucinated but Factual! Inspecting the Factuality of Hallucinations in Abstractive Summarization'
subtitle: ''
summary: ''
authors:
- Meng Cao
- Yue Dong
- Jackie Cheung
tags: []
categories: []
date: '2022-05-22'
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
abstract: 'State-of-the-art abstractive summarization systems often generate hallucinations; i.e., content that is not directly inferable from the source text. Despite being assumed to be incorrect, we find that much hallucinated content is actually consistent with world knowledge, which we call factual hallucinations. Including these factual hallucinations in a summary can be beneficial because they provide useful background information. In this work, we propose a novel detection approach that separates factual from non-factual hallucinations of entities. Our method is based on an entity’s prior and posterior probabilities according to pre-trained and finetuned masked language models, respectively. Empirical results suggest that our method vastly outperforms two baselines in both accuracy and F1 scores and has a strong correlation with human judgments on factuality classification tasks.Furthermore, we use our method as a reward signal to train a summarization system using an off-line reinforcement learning (RL) algorithm that can significantly improve the factuality of generated summaries while maintaining the level of abstractiveness.'
publication: '*Annual Meeting of the Association for Computational Linguistics (ACL)*'
links:
- name: Arxiv
  url: https://arxiv.org/pdf/2109.09784.pdf
- name: ACL Anthology
  url: https://aclanthology.org/2022.acl-long.236/
- name: Code
  url: https://github.com/mcao516/entfa
---
