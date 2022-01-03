---
# Documentation: https://wowchemy.com/docs/managing-content/

title: A Deeper Understanding of State-Based Critics in Multi-Agent Reinforcement Learning
  Learning
subtitle: ''
summary: 'We prove that state-based centralized critic is theoretically unsound. We also provide bias-variance trade-off analysis and empirical advice.'
authors:
- Xueguang Lyu
- Andrea Baisero
- Yuchen Xiao
- Christopher Amato
tags: []
categories: []
date: '2022-01-01'
lastmod: 2022-02-23T12:48:02-05:00
featured: true
draft: false
url_pdf: "https://arxiv.org/pdf/2102.04402.pdf"

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
publishDate: '2022-02-23T17:48:02.492153Z'
# publication_types:
# - '1'
abstract: 'Centralized Training for Decentralized Execution, where training is done in a centralized offline fashion, has become a popular solution paradigm in Multi-Agent Reinforcement Learning. Many such methods take the form of actor-critic with state-based critics, since centralized training allows access to the true system state, which can be useful during training despite not being available at execution time. State-based critics have become a common empirical choice, albeit one which has had limited theoretical justification or analysis. In this paper, we show that state-based critics can introduce bias in the policy gradient estimates, potentially undermining the asymptotic guarantees of the algorithm. We also show that, even if the state-based critics do not introduce any bias, they can still result in a larger gradient variance, contrary to the common intuition. Finally, we show the effects of the theories in practice by comparing different forms of centralized critics on a wide range of common benchmarks, and detail how various environmental properties are related to the effectiveness of different types of critics.
'
publication: 'In *Proceedings Thirty-Sixth AAAI Conference on Artificial Intelligence (AAAI-22)*'
publication_short: 'In *AAAI*'
---
