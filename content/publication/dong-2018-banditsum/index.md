---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'BanditSum: Extractive Summarization as a Contextual Bandit'
subtitle: ''
summary: ''
authors:
- Yue Dong
- Yikang Shen
- Eric Crawford
- Herke van Hoof
- Jackie Chi Kit Cheung
tags: []
categories: []
date: '2018-10-31'
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
abstract: 'In this work, we propose a novel method for training neural networks to perform single-document extractive summarization without heuristically-generated extractive labels. We call our approach BanditSum as it treats extractive summarization as a contextual bandit (CB) problem, where the model receives a document to summarize (the context), and chooses a sequence of sentences to include in the summary (the action). A policy gradient reinforcement learning algorithm is used to train the model to select sequences of sentences that maximize ROUGE score. We perform a series of experiments demonstrating that BanditSum is able to achieve ROUGE scores that are better than or comparable to the state-of-the-art for extractive summarization, and converges using significantly fewer update steps than competing approaches. In addition, we show empirically that BanditSum performs significantly better than competing approaches when good summary sentences appear late in the source document.'
publication: '*Empirical Methods of Natural Language Processing (EMNLP)*'
links:
- name: Arxiv
  url: https://arxiv.org/abs/1809.09672
- name: ACL Anthology
  url: https://aclanthology.org/D18-1409/
- name: Code
  url: https://github.com/YueDongCS/BanditSum
- name: Video
  url: https://vimeo.com/306160623
---
