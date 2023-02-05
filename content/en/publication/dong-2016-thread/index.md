---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Threaded ensembles of supervised and unsupervised neural networks for stream learning'
subtitle: ''
summary: ''
authors:
- Yue Dong
- Nathalie Japkowicz
tags: [[<span style="color:red"> **Best Paper Award** </span>]]
categories: []
date: '2016-05-13'
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
abstract: 'Most existing model-based approaches to anomaly detection in streaming data are based on decision trees due to their fast construction speed [1]. This paper proposes two fast anomaly detectors based on ensembles of neural networks for evolving data streams. One model is a supervised online learning algorithm involving an ensemble of threaded multilayer perceptrons (MLP). The other model is a one-class learning algorithm with an ensemble of threaded autoencoders. The latter model only requires data from the positive class for training and is accurate even when anomalous training data are rare. The models feature an ensemble of multilayer perceptrons or autoencoders from multi-threads which evolve with data streams. Using multi-threads makes the methods highly efficient because both methods process data streams in parallel. Our analysis shows that both methods in streaming data have constant small time complexity and constant memory requirement. When compared with Very Fast Decision Trees (VFDT), a state-of-the-art algorithm, our methods performed favorably in terms of detection accuracy and training time for the datasets under consideration.'
publication: '*Canadian conference on artificial intelligence*'
links:
- name: Paper
  url: https://link.springer.com/chapter/10.1007/978-3-319-34111-8_37
- name: Best Paper Award
  url: 
---
