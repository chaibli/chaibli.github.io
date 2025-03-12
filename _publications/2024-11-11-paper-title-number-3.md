---
title: "REM: Enabling Real-Time Neural-Enhanced Video Streaming on Mobile Devices Using Macroblock-Aware Lookup Table"
collection: publications
permalink: /publication/2024-11-11-paper-title-number-3
excerpt: '__Baili Chai__, Di Wu, Jinyu Chen, Mengyu Yang, Zelong Wang, Miao Hu'
date: 2024-11-1
venue: 'IEEE Transactions on Mobile Computing (TMC), CCF-A'
---

<img src="https://i.imgur.com/od2WAtA.png" width="100%">

In this [paper](https://ieeexplore.ieee.org/document/10750425), we propose REM, a novel neural-enhanced mobile video streaming framework. REM utilizes a customized lookup table to facilitate real-time neuralenhanced video streaming on mobile devices. Initially, we conduct a series of measurements to identify abundant macroblock redundancies across frames in a video stream. Subsequently, we introduce a dynamic macroblock selection algorithm that prioritizes important macroblocks for neural enhancement. The SR-enhanced results are stored in the lookup table and efficiently reused to meet real-time requirements and minimize resource overhead. By considering macroblock-level characteristics of the video frames,
the lookup table enables efficient and fast processing. Additionally, we design a lightweight macroblock-aware SR module to expedite inference. 

Finally, we perform extensive experiments on various mobile devices. The results demonstrate that REM enhances overall processing throughput by up to 10.2 times and reduces power consumption by up to 58.6% compared to state-of-the-art methods. Consequently, this leads to a 38.06% improvement in the quality of experience for mobile users.