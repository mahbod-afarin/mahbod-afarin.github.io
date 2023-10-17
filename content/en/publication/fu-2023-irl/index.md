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
abstract: 'Current state-of-the-art summarization models are trained with either maximum likelihood estimation (MLE) or reinforcement learning (RL). In this study, we investigate the third training paradigm and argue that inverse reinforcement learning (IRL) may be more suitable for text summarization. IRL focuses on estimating the reward function of an agent, given a set of observations of that agent's behavior. Generally, IRL provides advantages in situations where the reward function is not explicitly known or where it is difficult to define or interact with the environment directly. These situations are exactly what we observe in summarization. Thus, we introduce inverse reinforcement learning into text summarization and define a suite of sub-rewards that are important for summarization optimization. By simultaneously estimating the reward function and optimizing the summarization agent with expert demonstrations, we show that the model trained with IRL produces summaries that closely follow human behavior, in terms of better ROUGE, coverage, novelty, compression ratio and factuality when compared to the baselines trained with MLE and RL.'
publication: '*Findings of Empirical Methods of Natural Language Processing (EMNLP)*'
links:
- name: Arxiv
  url: https://arxiv.org/abs/2212.09917
- name: ACL Anthology
  url: https://arxiv.org/abs/2212.09917
---
