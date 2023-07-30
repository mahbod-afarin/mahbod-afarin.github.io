---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Plug and Pray: Exploiting off-the-shelf components of Multi-Modal Models'
subtitle: ''
summary: ''
authors:
- Erfan Shayegani
- Yue Dong
- Nael Abu-Ghazaleh
tags: []
categories: []
date: '2020-11-16'
lastmod: 2023-07-18T19:57:59-04:00
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
publishDate: '2023-07-18T23:57:59.485338Z'
publication_types:
- '1'
abstract: 'The rapid growth and increasing popularity of incorporating additional modalities (e.g., vision) into large language models (LLMs) has raised significant security concerns. This expansion of modality, akin to adding more doors to a house, unintentionally creates multiple access points for adversarial attacks. In this paper, by introducing adversarial embedding space attacks, we emphasize the vulnerabilities present in multi-modal systems that originate from incorporating off-the-shelf components like public pre-trained encoders in a plug-and-play manner into these systems. In contrast to existing work, our approach does not require access to the multi-modal system's weights or parameters but instead relies on the huge under-explored embedding space of such pre-trained encoders. Our proposed embedding space attacks involve seeking input images that reside within the dangerous or targeted regions of the extensive embedding space of these pre-trained components. These crafted adversarial images pose two major threats: 'Context Contamination' and 'Hidden Prompt Injection'-both of which can compromise multi-modal models like LLaVA and fully change the behavior of the associated language model. Our findings emphasize the need for a comprehensive examination of the underlying components, particularly pre-trained encoders, before incorporating them into systems in a plug-and-play manner to ensure robust security.'
publication: '*In submission*'
links:
 - name: arXiv
  url: https://arxiv.org/abs/2307.13808
# - name: ACL Anthology
#  url: https://aclanthology.org/2020.emnlp-main.506/
# - name: Code
#  url: https://github.com/mcao516/Factual-Error-Correction
# - name: Video
#  url: https://slideslive.com/38939120/factual-error-correction-for-abstractive-summarization-models
---
