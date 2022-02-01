---
slides: example
url_pdf: ""
summary: An example of using the in-built project page.
url_video: ""
date: 2016-04-27T00:00:00Z
external_link: ""
url_slides: ""
title: Vertebral Landmark Detection
tags:
  - Deep Learning
links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/georgecushen
image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart
url_code: ""
---
Brief introduction: estimating the locations of corner/center landmarks for each vertebra on anterior-posteriorspine X-ray images ( thoracic and lumbar spine, 17 vertebrae per image)

* Basic Architecture: heatmap-based pose estimation algorithm (backbone: HRNet)  Multi-head mechanism: calculating corner offset with regard to center points after calibrating center land-mark predictions, which are extracted from the 17-channel center heatm







![]()