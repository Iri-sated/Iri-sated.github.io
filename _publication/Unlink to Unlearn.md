---
title: "Unlink to Unlearn: Simplifying Edge Unlearning in GNNs"
excerpt: "(WWW' 2024) Jiajun Tan, Fei Sun, Ruichen Qiu, Du Su, Huawei Shen"
type: publication
layout: single
author_profile: true
#toc: true
---
[GitHub](https://github.com/Sumsky21/Unlink-to-Unlearn){: .btn .btn--primary}
[arXiv](https://arxiv.org/abs/2402.10695){: .btn .btn--danger}

As concerns over data privacy intensify, unlearning in Graph Neural Networks (GNNs) has emerged as a prominent research frontier in academia. This concept is pivotal in enforcing the *right to be forgotten*, which entails the selective removal of specific data from trained GNNs upon user request. Our research focuses on edge unlearning, a process of particular relevance to real-world applications. Current state-of-the-art approaches like GNNDelete can eliminate the influence of specific edges yet suffer from *over-forgetting*, which means the unlearning process inadvertently removes excessive information beyond needed, leading to a significant performance decline for remaining edges. Our analysis identifies the loss functions of GNNDelete as the primary source of over-forgetting and also suggests that loss functions may be redundant for effective edge unlearning. Building on these insights, we simplify GNNDelete to develop **Unlink to Unlearn** (UtU), a novel method that facilitates unlearning exclusively through unlinking the forget edges from graph structure. Our extensive experiments demonstrate that UtU delivers privacy protection on par with that of a retrained model while preserving high accuracy in downstream tasks, by upholding over 97.3% of the retrained model's privacy protection capabilities and 99.8% of its link prediction accuracy. Meanwhile, UtU requires only constant computational demands, underscoring its advantage as a highly lightweight and practical edge unlearning solution.