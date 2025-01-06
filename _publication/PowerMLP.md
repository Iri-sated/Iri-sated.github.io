---
title: "PowerMLP: An Efficient Version of KAN"
excerpt: "(AAAI' 2025) Ruichen Qiu, Yibo Miao, Shiwen Wang, Lijia Yu, Yifan Zhu, Xiao-Shan Gao"
type: publication
layout: single
author_profile: true
#toc: true
---
[GitHub](){: .btn .btn--primary}
[arXiv](https://arxiv.org/abs/2412.13571v1){: .btn .btn--danger}

The Kolmogorov-Arnold Network (KAN) is a new network architecture known for its high accuracy in several tasks such as function fitting and PDE solving. The superior expressive capability of KAN arises from the Kolmogorov-Arnold representation theorem and learnable spline functions. However, the computation of spline functions involves multiple iterations, which renders KAN significantly slower than MLP, thereby increasing the cost associated with model training and deployment. The authors of KAN have also noted that "the biggest bottleneck of KANs lies in its slow training. KANs are usually 10x slower than MLPs, given the same number of parameters." To address this issue, we propose a novel MLP-type neural network PowerMLP that employs simpler non-iterative spline function representation, offering approximately the same training time as MLP while theoretically demonstrating stronger expressive power than KAN. Furthermore, we compare the FLOPs of KAN and PowerMLP, quantifying the faster computation speed of PowerMLP. Our comprehensive experiments demonstrate that PowerMLP generally achieves higher accuracy and a training speed about 40 times faster than KAN in various tasks.