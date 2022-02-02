---
title: Few-shot learning for cardiac arrhythmia classification
date: 2021-03-05T15:03:00.000Z
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

Then we proposed a metric-based meta-transfer scheme.  Different from standard metric-based meta-learning algorithms, such as [PrototyNet](https://arxiv.org/abs/1703.05175), we used the auxiliary dataset from PTB diagnostic database to pretrain the feature extractor at first by implementing binary classification task (categorize into ill or healthy cases).  Then we transfered this prior knowledge into the few-shot learning on MIT-BIH dataset  of 5 classes (healthy cases and 4 specific cardiac arrhythmia types). 

![](screenshot-20220202-192225.png)

I programmed the proposed method and conducted extensive experiments. We demonstrated that with the proposed meta-transfer scheme, our method outperforms other comparative methods in terms of accuracy when handling various few-shot tasks. Finally, we published it on *[Digital Signal Processing](https://www.sciencedirect.com/science/article/pii/S1051200421001330)*.