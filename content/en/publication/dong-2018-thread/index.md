---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Threaded ensembles of autoencoders for stream learning'
subtitle: ''
summary: ''
authors:
- Yue Dong
- Nathalie Japkowicz
tags: []
categories: []
date: '2018-01-31'
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
- '2'
abstract: 'Anomaly detection in streaming data is an important problem in numerous application domains. Most existing model-based approaches to stream learning are based on decision trees due to their fast construction speed. This paper introduces streaming autoencoder (SA), a fast and novel anomaly detection algorithm based on ensembles of neural networks for evolving data streams. It is a one-class learner, which only requires data from the positive class for training and is accurate even when anomalous training data are rare. It features an ensemble of threaded autoencoders with continuous learning capacity. Furthermore, the SA uses a 2-step detection mechanism to ensure that real anomalies are detected with low false-positive rates. The method is highly efficient because it processes data streams in parallel with multithreads and alternating buffers. Our analysis shows that SA has a linear runtime and requires constant memory space. Empirical comparisons to the state-of-the-art methods on multiple benchmark data sets demonstrate that the proposed method detects anomalies efficiently with fewer false alarms.'
publication: '*Computational Intelligence*'
links:
- name: Paper
  url: https://onlinelibrary.wiley.com/doi/abs/10.1111/coin.12146
---
