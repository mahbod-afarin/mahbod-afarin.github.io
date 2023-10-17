---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Factual Error Correction for Abstractive Summarization Models'
subtitle: ''
summary: ''
authors:
- Yu Fu
- Deyi Xiong
- Yue Dong
tags: []
categories: []
date: '2023-10-16'
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
abstract: 'Despite recent advances in abstractive summarization, current summarization systems still suffer from content hallucinations where models generate text that is either irrelevant or contradictory to the source document. However, prior work has been predicated on the assumption that any generated facts not appearing explicitly in the source are undesired hallucinations. Methods have been proposed to address this scenario by ultimately improving faithfulness to the source document, but in reality, there is a large portion of entities in the gold reference targets that are not directly in the source. In this work, we show that these entities are not aberrations, but they instead require utilizing external world knowledge to infer reasoning paths from entities in the source. We show that by utilizing an external knowledge base, we can improve the faithfulness of summaries without simply making them more extractive, and additionally, we show that external knowledge bases linked from the source can benefit the factuality of generated summaries.'
publication: '*Findings of Empirical Methods of Natural Language Processing (Findings of EMNLP)*'
links:
- name: Arxiv
  url: https://arxiv.org/abs/2204.13761
- name: ACL Anthology
  url: https://arxiv.org/abs/2204.13761
---
