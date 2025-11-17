---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Install OpenAI Gym with Atari on macOS"
subtitle: ""
summary: "Quick guide to installing OpenAI Gym with Atari environments on macOS using brew and pip."
authors: []
tags: []
categories: ["environment setup"]
date: 2018-09-23T13:46:11-05:00
lastmod: 2018-09-23T13:46:11-05:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  placement: 2
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

![image](https://miro.medium.com/max/1232/1*guXWQC5Qetu_WdmJwdpJ4w.png)

It’s simple: install cmake and zlib first, and then install gym and atari environment on macOS.

```[bash]
brew install cmake zlib
pip install 'gym[atari]'
```

The quotation marks are for people who are using zsh.
If you want all environments provided by OpenAI Gym, you can install `gym[all]`.

Enjoy your games.
