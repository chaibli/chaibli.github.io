---
title: "Masked360: Enabling Robust 360-degree Video Streaming with Ultra Low Bandwidth Consumption"
collection: publications
permalink: /publication/2023-02-22-paper-title-number-1
excerpt: 'Zhenxiao Luo, __Baili Chai__, Zelong Wang, Miao Hu, Di Wu'
date: 2023-02-22
venue: 'IEEE Transactions on Visualization and Computer Graphics (TVCG), CCF-A'
---

<img src="https://i.imgur.com/ByOmr44.png" width="100%">

In this [paper](https://ieeexplore.ieee.org/document/10049727), we propose a practical neural-enhanced 360-degree video streaming framework called Masked360, which can significantly reduce bandwidth consumption and achieve robustness against packet loss. 

In Masked360, instead of transmitting the complete video frame, the video server only transmits a masked low-resolution version of each video frame to reduce bandwidth significantly. When delivering masked video frames, the video server also sends a lightweight neural network model called MaskedEncoder to clients. Upon receiving masked frames, the client can reconstruct the original 360-degree video frames and start playback. To further improve the quality of video streaming, we also propose a set of optimization techniques, such as complexity-based patch selection, quarter masking strategy, redundant patch transmission and enhanced model training methods. 

In addition to bandwidth savings, Masked360 is also robust to packet loss during the transmission, because packet losses can be concealed by the reconstruction operation performed by the MaskedEncoder. Finally, we implement the whole Masked360 framework and evaluate its performance using real datasets. 

The experimental results show that Masked360 can achieve 4K 360-degree video streaming with bandwidth as low as 2.4 Mbps. Besides, video quality of Masked360 is also improved significantly, with an improvement of 5.24-16.61% in terms of PSNR and 4.74-16.15% in terms of SSIM compared to other baselines.
