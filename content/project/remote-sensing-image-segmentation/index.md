---
title: "Remote sensing image segmentation "
date: 2022-02-01T15:06:26.563Z
summary: "**Brief introduction:** a track of 2020 CCF BDCI Competition,
  implementing a 7-class semantic segmentation task on remote sensing images
  (leader of a 5-member team)"
draft: false
featured: false
tags:
  - Computer Vision
categories:
  - Computer Vision
image:
  filename: ""
  focal_point: Smart
  preview_only: false
---
The theme of this competition is to segment remote sensing images and classify different parts into 7 types of landforms, such as lanes, water, or grassland. 

We adopted the powerful semantic segmentation method, DeepLabv3+ with the backbone of ResNet101 on the training dataset of 140,000 images and the testB set of 20,000 images.

For better generalization performance and representation power of the method, I added two types of attention blocks, channel attention and spatial attention, to focus on more task-relevant channels and spatial areas.

![](screenshot-20220202-223721.png "Attention Blocks")

For tackling the class-imbalance problem, I used the weighted sum of the Weighted Cross-Entropy Loss and Lovasz Softmax Loss for training.

![](screenshot-20220202-222817.png)

Besides, I also chose samples of minor classes, i.e., lane and grassland to construct independent U-Net -based binary classifiers and merged the results with the original predictions of the DeepLab model.

![](图片6.png)

After using ensemble strategies, and adopting dilation and corrosion as post-processing steps, we ranked 9/116 on the Rank B board in the 1st Round and ended with 12/28 on the Rank B board in the 2nd Round.