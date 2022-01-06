---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Likelihood Quantile Networks for Coordinating Multi-Agent Reinforcement Learning
subtitle: ''
summary: ''
authors:
- Xueguang Lyu
- Christopher Amato
tags: []
categories: []
date: '2020-01-01'
lastmod: 2021-02-23T12:48:02-05:00
featured: false
draft: false
url_pdf: "https://arxiv.org/pdf/1812.06319.pdf"
# author_notes:
# - "Equal contribution"
# - "Equal contribution"


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
publishDate: '2021-02-23T17:48:02.259137Z'
publication_types:
- '1'
abstract: "When multiple agents learn in a decentralized manner, the environment appears non-stationary from the perspective of an individual agent due to the exploration and learning of the other agents. Recently proposed deep multi-agent reinforcement learning methods have tried to mitigate this non-stationarity by attempting to determine which samples are from other agent exploration or suboptimality and take them less into account during learning. Based on the same philosophy, this paper introduces a decentralized quantile estimator, which aims to improve performance by distinguishing non-stationary samples based on the likelihood of returns. In particular, each agent considers the likelihood that other agent exploration and policy changes are occurring, essentially utilizing the agents' own estimations to weigh the learning rate that should be applied towards the given samples. We introduce a formal method of calculating differences of our return distribution representations and methods for utilizing it to guide updates. We also explore the effect of risk-seeking strategies for adjusting learning over time and propose adaptive risk distortion functions which guides risk sensitivity. Our experiments, on traditional benchmarks and new domains, show our methods are more stable, sample efficient and more likely to converge to a joint optimal policy than previous methods."


publication: 'In *Proceedings of the 19th International Conference on Autonomous Agents and MultiAgent Systems*'

publication_short: In *AAMAS*


---
