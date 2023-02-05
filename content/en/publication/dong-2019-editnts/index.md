---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'EditNTS: An Neural Programmer-Interpreter Model for Sentence Simplification through Explicit Editing'
subtitle: ''
summary: ''
authors:
- Yue Dong
- Zichao Li
- Mehdi Rezagholizadeh
- Jackie Chi Kit Cheung
tags: []
categories: []
date: '2019-07-28'
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
abstract: 'We present the first sentence simplification model that learns explicit edit operations (ADD, DELETE, and KEEP) via a neural programmer-interpreter approach. Most current neural sentence simplification systems are variants of sequence-to-sequence models adopted from machine translation. These methods learn to simplify sentences as a byproduct of the fact that they are trained on complex-simple sentence pairs. By contrast, our neural programmer-interpreter is directly trained to predict explicit edit operations on targeted parts of the input sentence, resembling the way that humans perform simplification and revision. Our model outperforms previous state-of-the-art neural sentence simplification models (without external knowledge) by large margins on three benchmark text simplification corpora in terms of SARI (+0.95 WikiLarge, +1.89 WikiSmall, +1.41 Newsela), and is judged by humans to produce overall better and simpler output sentences.'
publication: '*Annual Meeting of the Association for Computational Linguistics (ACL)*'
links:
- name: Arxiv
  url: https://arxiv.org/abs/1906.08104
- name: ACL Anthology
  url: https://aclanthology.org/P19-1331/
- name: Code
  url: https://github.com/YueDongCS/EditNTS
- name: Video
  url: https://vimeo.com/384771870
---
