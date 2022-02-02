---
title: Inference acceleration for indecent image classification
date: 2022-02-01T15:07:52.260Z
summary: "Brief introduction: filtering indecent images on Internet by
  implementing a 6-class image classification task, the aim is to reduce the
  inference latency without sacrificing accuracy for further employment on edge
  devices."
draft: false
featured: false
tags:
  - Efficient Machine Learning
categories:
  - Efficient Machine Learning
image:
  filename: ""
  focal_point: Smart
  preview_only: false
---
Due to the limited computational resources of the edge devices, the efficiency of ML methods is important for employment. The objective of improving computational efficiency is to reduce the average latency while maintaining accuracy. 

Our solution was employing an adaptive inference scheme with dynamic neural networks. For this 6-class image classification task, I employ the novel spatially adaptive inference framework, [GFNet](https://proceedings.neurips.cc/paper/2020/file/1963bd5135521d623f6c29e6b1174975-Paper.pdf), proposed by our Leap Lab. 

![](self-introduction_yukang-yang_-tsinghua-university~2.gif)

While maintaining the accuracy of 97.06%, I reduced the average latency by nearly 75% and will further deploy on phones.