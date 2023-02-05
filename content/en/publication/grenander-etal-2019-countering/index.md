---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Countering the Effects of Lead Bias in News Summarization via Multi-Stage Training and Auxiliary Losses'
subtitle: ''
summary: ''
authors:
- Matt Grenander
- Yue Dong
- Jackie Chi Kit Cheung
- Annie Louis

tags: []
categories: []
date: '2019-11-03'
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
abstract: 'Sentence position is a strong feature for news summarization, since the lead often (but not always) summarizes the key points of the article. In this paper, we show that recent neural systems excessively exploit this trend, which although powerful for many inputs, is also detrimental when summarizing documents where important content should be extracted from later parts of the article. We propose two techniques to make systems sensitive to the importance of content in different parts of the article. The first technique employs ‘unbiased’ data; i.e., randomly shuffled sentences of the source document, to pretrain the model. The second technique uses an auxiliary ROUGE-based loss that encourages the model to distribute importance scores throughout a document by mimicking sentence-level ROUGE scores on the training data. We show that these techniques significantly improve the performance of a competitive reinforcement learning based extractive system, with the auxiliary loss being more powerful than pretraining.'
publication: '*Empirical Methods of Natural Language Processing (EMNLP)*'
links:
- name: Arxiv
  url: https://arxiv.org/abs/1909.04028
- name: ACL Anthology
  url: https://aclanthology.org/D19-1620/
---
