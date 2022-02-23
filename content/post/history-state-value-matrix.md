---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "The History-State Value Matrix"
subtitle: "Understanding the relationship between history values and state values."
summary: "This blog gives a graphical illustration of how history-state values are related with biases with state-based critics."
authors:
- Xueguang Lyu
tags: []
categories: []
date: 2022-02-23T12:57:44-05:00
lastmod: 2022-02-23T12:57:44-05:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

This blog discuss the bias seen in [A Deeper Understanding of State-Based Critics in Multi-Agent Reinforcement Learning]({{< ref "/publication/lyu-2022-a" >}} "A Deeper Understanding of State-Based Critics in Multi-Agent Reinforcement Learning").

The history-state values $Q(h,s,a)$ are defined as the expected return given the agent in state $s$, with history $h$ and taking an $a$.
If we only consider one action particular action (say $a_o$), we get a matrix of values that correspond to different states and histories .

<img src="/history-state-value-matrix/hsv.png" alt="drawing" width="300"/>

When we consider the expected value for a certain history or a certain state, we are implicitly taking an average over a certain column or a certain row respectively:

<img src="/history-state-value-matrix/hv_and_sv.png" alt="drawing" width="700"/>


If we are to use state values to approximate history values in the fashion seen in state-based critics nowadays, say $\boldsymbol{h}_1$,
we should be expecting to use the values from one single column as shown:

<img src="/history-state-value-matrix/h1.png" alt="drawing" width="300"/>


The catch, however, is that the state values being used here are themselves averages from entires rows

<img src="/history-state-value-matrix/h1s.png" alt="drawing" width="300"/>

So in essence, this value approximation for $\boldsymbol{h}_1$ becomes a weighted sum of the *entire* matrix.

<img src="/history-state-value-matrix/h1sh.png" alt="drawing" width="400"/>

As such, we conclude that using the state values to approximate history values is flawed.

<img src="/history-state-value-matrix/unequal.png" alt="drawing" width="600"/>

There is a notable special case, though. Now think about it, for our approximation to be not biased, we would just need the yellow part to not interfere our mean (duh).

<img src="/history-state-value-matrix/yellow.png" alt="drawing" width="300"/>

So when would this happen? Errrrr... Every row have the same value? Yes, that should do it!
And it so happens it is the case for having more information or less information does not matter from a value equivalent standpoint.
And it is also the case with some benchmarks seen in the paper.
