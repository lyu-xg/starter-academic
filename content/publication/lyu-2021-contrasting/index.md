---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Contrasting Centralized and Decentralized Critics in Multi-Agent Reinforcement
  Learning
subtitle: ''
summary: 'We prove and test that centralized critic and decentralized critic in multi-agent learning is asymptotically equivalent. We also provide bias-variance trade-off analysis and empirical advice.'
authors:
- Xueguang Lyu
- Yuchen Xiao
- Brett Daley
- Christopher Amato
tags: []
categories: []
date: '2021-01-01'
lastmod: 2021-02-23T12:48:02-05:00
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
publishDate: '2021-02-23T17:48:02.492153Z'
publication_types:
- '1'
abstract: 'Centralized Training for Decentralized Execution, where agents are trained offline using centralized information but execute in a decentralized manner online, has gained popularity in the multi-agent reinforcement learning community. In particular, actor-critic methods with a centralized critic and decentralized actors are a common instance of this idea. However, the implications of using a centralized critic in this context are not fully discussed and understood even though it is the standard choice of many algorithms. We therefore formally analyze centralized and decentralized critic approaches, providing a deeper understanding of the implications of critic choice. Because our theory makes unrealistic assumptions, we also empirically compare the centralized and decentralized critic methods over a wide set of environments to validate our theories and to provide practical advice. We show that there exist misconceptions regarding centralized critics in the current literature and show that the centralized critic design is not strictly beneficial, but rather both centralized and decentralized critics have different pros and cons that should be taken into account by algorithm designers.'
publication: 'In *Proceedings of the 20th International Conference on Autonomous Agents and MultiAgent Systems*'
publication_short: 'In *AAMAS*, Best Paper Award Finalist'
---
