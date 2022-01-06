---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Local Advantage Actor-Critic for Robust Multi-Agent Deep Reinforcement Learning"
authors: 
- Yuchen Xiao
- Xueguang Lyu
- Christopher Amato
date: 2021-11-04T16:25:00-05:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2021-11-04T16:25:00-05:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "In *2021 International Symposium on Multi-Robot and Multi-Agent Systems*"
publication_short: "In *MRS*"

abstract: "Policy gradient methods have become popular in multi-agent reinforcement learning, but they suffer from high variance due to the presence of environmental stochasticity and exploring agents (i.e., non-stationarity), which is potentially worsened by the difficulty in credit assignment. As a result, there is a need for a method that is not only capable of efficiently solving the above two problems but also robust enough to solve a variety of tasks. To this end, we propose a new multi-agent policy gradient method, called Robust Local Advantage (ROLA) Actor-Critic. ROLA allows each agent to learn an individual action-value function as a local critic as well as ameliorating environment non-stationarity via a novel centralized training approach based on a centralized critic. By using this local critic, each agent calculates a baseline to reduce variance on its policy gradient estimation, which results in an expected advantage action-value over other agents’ choices that implicitly improves credit assignment. We evaluate ROLA across diverse benchmarks and show its robustness and effectiveness over a number of state-of-the-art multi-agent policy gradient algorithms."

# Summary. An optional shortened abstract.
summary: ""

tags: []
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_pdf: "https://arxiv.org/pdf/2110.08642.pdf"
url_code:
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
