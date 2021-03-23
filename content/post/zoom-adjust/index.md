---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "How can you remove the transcription side panel in Zoom Recordings"
subtitle: ""
summary: "View zoom recording without distraction"
authors: []
tags: []
categories: []
date: 2020-11-13T13:51:09-05:00
lastmod: 2020-11-13T13:51:09-05:00
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
I found having a transcript on the side of the video is very annoying because the changing text catches my attention rampantly especially when the content is very difficult to grasp.

![image](https://miro.medium.com/max/4800/1*jS3-OB62UPMZkDhdbC9anQ.jpeg)

Therefore I wrote a little script to remove the transcripts.

```[javascript]
document.getElementsByClassName('player-panel-r')[0].removeChild(document.getElementsByClassName('transcript-wrapper')[0])
document.getElementsByClassName('player-view-wrapper')[0].setAttribute('style', 'width: 100%;')
```

You can sort of tell that, after being ran in browser console, It will remove the transcript section and enlarge the video section for you.
You have also use extensions such as [Script Runner](https://addons.mozilla.org/en-US/firefox/addon/scripts-runner/) that run custom JS with a shortcut button.

![image_after_adjustment](https://miro.medium.com/max/4800/1*40eddmxEfBcQmpK_6Nw56A.jpeg)
