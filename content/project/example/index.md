---
slides: example
url_pdf: ""
summary: detecting vertebral landmarks for the diagnosis of scoliosis
url_video: ""
date: 2016-04-27T00:00:00.000Z
external_link: ""
url_slides: ""
title: Vertebral Landmark Detection
tags:
  - Deep Learning
links: null
image:
  caption: ""
  focal_point: ""
url_code: ""
---
Brief introduction: estimating the locations of corner/center landmarks for each vertebra on anterior-posteriorspine X-ray images ( thoracic and lumbar spine, 17 vertebrae per image)

* Basic Architecture: heatmap-based pose estimation algorithm (backbone: HRNet) 
  Multi-head mechanism: calculating corner offset with regard to center points after calibrating center land-mark predictions, which are extracted from the 17-channel center heatm







![]()
