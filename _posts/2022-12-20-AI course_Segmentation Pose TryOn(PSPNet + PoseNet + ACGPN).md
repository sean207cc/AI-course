---
layout: post
title: AI course_Segmentation Pose TryOn(PSPNet + PoseNet + ACGPN)
author: [Sean Liu,李宥諭]
category: [Lecture]
tags: [jekyll, ai]
---
期末專題實作: Segmentation Pose Try-On (試穿衣服)

---
## Segmentation Pose Try-On (試穿衣服)
Go to [Segmentation Pose Try-On (試穿衣服)](https://www.kaggle.com/code/seeanbooo/segmentation-pose-tryon) click [Fork] <br />

### 系統簡介及功能說明

1. **系統簡介**:<br>
   訓練並利用生成式對抗網路以及pose map來辨識圖片中的人物的衣服及肢體並且替換衣服

2. **功能說明**:<br>
   替換圖片中人物的衣服來達到不用走出門在家就可以試穿衣服的目的，對於交通不便捷的地區或行動不方便的人來說，在家也能盡情的試穿網購網站的衣服

---
### 系統方塊圖
![](https://github.com/sean207cc/AI-course/blob/gh-pages/images/截圖%202023-01-06%20下午4.46.36.png?raw=true)

**AI模型說明**:<br>
先通過 Expansion layer 來擴展維度，之後再用深度可分離卷積來提取特徵，之後使用 Projection layer 來壓縮數據，讓網路重新變小。因為 Expansion layer 和 Projection layer 都是有可以學習的參數，所以整個網路結構可以學習到如何更好的擴展數據和重新壓縮數據。
<iframe width="560" height="315" src="https://www.youtube.com/embed/TEXL9gsCksQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### 製作步驟

1. 建立資料集 dataset
2. 移植程式to Kaggle
3. Kaggle上訓練模型
4. Kaggle上測試模型

---
### 系統測試及成果展示
![](https://github.com/sean207cc/AI-course/blob/gh-pages/images/show%201.png?raw=true)
![](https://github.com/sean207cc/AI-course/blob/gh-pages/images/show%202.png?raw=true)
![](https://github.com/sean207cc/AI-course/blob/gh-pages/images/show%203.png?raw=true)
<iframe width="560" height="315" src="https://www.youtube.com/embed/AwWavQFB7ds" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Go to [Segmentation Pose Try-On (試穿衣服)](https://www.kaggle.com/code/seeanbooo/segmentation-pose-tryon) click [Fork] <br />

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*
