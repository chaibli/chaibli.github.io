---
title: "SDSR: Optimizing Metaverse Video Streaming via Saliency-driven Dynamic Super-Resolution"
collection: publications
permalink: /publication/2023-12-21-paper-title-number-2
excerpt: '__Baili Chai__, Jinyu Chen, Zhenxiao Luo, Zelong Wang, Miao Hu, Yipeng Zhou, Di Wu'
date: 2023-12-21
venue: 'IEEE Journal on Selected Areas in Communications (JSAC), CCF-A'
---

<img src="https://i.imgur.com/mHxX7Uj.png" width="100%">

In this [paper](https://ieeexplore.ieee.org/document/10368051), we first conduct a dedicated measurement study to unveil the impact of different granularities of SR models. It is found that the scene of a video largely determines the effectiveness of SR models in different granularities. 

Based on our observations, we propose a novel 360-degree video streaming framework with saliency-driven dynamic super-resolution, called SDSR. To maximize user QoE, we formally formulate an optimization problem and adopt the model predictive control (MPC) theory for bitrate adaptation and SR model selection. To improve the effectiveness of SR model, we leverage the saliency information, which well reflects users’ view interests, for model training. In addition, we reuse an SR model for similar chunks based on temporal redundancy of a video. 

Finally, we conduct extensive experiments on real traces and the results show that SDSR outperforms the state-of-the-art algorithms with an improvement up to 32.78% in terms of the average QoE.