---
title: Few-shot learning for cardiac arrhythmia classification
date: 2022-02-01T15:03:48.016Z
summary: "**Brief introduction:** few-shot learning problem for cardiac
  arrhythmia classification with the ECG signal collected from the wearable
  devices to employ AI edge computing."
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


Typically, we use ECG signals to diagnose the type of cardiac arrhythmia. This classification problem could be solved with the help of machine learning methods. Nowadays wearable devices like smartwatches can track and report vital heart signs. However, most of them lack real-time disease prediction. For more intelligent health monitoring, we would like to employ ML methods on these edge devices. Constrained by the data storage of these devices,  we are facing a few-shot learning problem. 

First, we process the ECG signal into 2D spectrograms by using short-time Fourier transform (STFT).

![](screenshot-20220202-184432.png)

Then we proposed a meta-transfer scheme.

![](screenshot-20220202-192225.png)