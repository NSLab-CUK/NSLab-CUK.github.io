---
layout: post
title:  DegFairGT, A Novel Graph Transformer Model for Learning Fair Representations
date:   2025-04-22 00:00:00 +0900
image:  Bib_Network.png
tags:   Release
published: true
description: The Network Science Lab at the Catholic University of Korea releases Degree Fairness Graph Transformer, namely DegFairGT, a novel Graph Transformer model specialised in learning fair representations.
---

We present [DegFairGT](https://github.com/NSLab-CUK/Community-aware-Graph-Transformer), a novel Graph Transformer model specialised in learning fair representations though learnable structural augmentation and structural self-attention and developed by NS Lab, CUK based on pure PyTorch backend. This paper has been accepted for publication in IEEE Transactions on Network Science and Engineering.

<p align="center">
  <img src="/images/CGT.jpg" alt="Graph Transformer Architecture" width="800">
  <br>
  <b></b> The overall architecture of DegFairGT.
</p>

Graph Neural Networks (GNNs) update node representations through message passing, which is primarily based on the homophily principle, assuming that adjacent nodes share similar features. However, in real-world graphs with long-tailed degree distributions, high-degree nodes dominate message passing, causing a degree bias where low-degree nodes remain under-represented due to inadequate messages. The main challenge in addressing degree bias is how to discover non-adjacent nodes to provide additional messages to low-degree nodes while reducing excessive messages for high-degree nodes. Nevertheless, exploiting non-adjacent nodes to provide valuable messages is challenging, as it could generate noisy information and disrupt the original graph structures. To solve it, we propose a novel Degree Fairness Graph Transformer, named **DegFairGT**, to mitigate degree bias by discovering structural similarities between non-adjacent nodes through learnable structural augmentation and structural self-attention. Our key idea is to exploit non-adjacent nodes with similar roles in the same community to generate informative edges under our augmentation, which could provide informative messages between nodes with similar roles while ensuring that the homophily principle is maintained within the community. To enable **DegFairGT** to learn such structural similarities, we then propose a structural self-attention to capture the similarities between node pairs. To preserve global graph structures and prevent graph augmentation from hindering graph structure, we propose a Self-Supervised Learning task to preserve p-step transition probability and regularize graph augmentation. Extensive experiments on six datasets showed that **DegFairGT** outperformed state-of-the-art baselines in degree fairness analysis, node classification, and node clustering tasks.


## A short description of **DegFairGT**:

- DegFairGT could exploit non-adjacent nodes with similar roles in the same community to generate informative edges under our augmentation, which could provide informative messages between nodes with similar roles while ensuring that the homophily principle is maintained within the community.
- We propose a novel graph transformer with improved self-attention that takes the augmented graph as input and encodes the within-community proximity into dot product self-attention and the roles of nodes. It is worth noting that we directly encode the high-order proximity into full dot product attention, which could enable **DegFairGT** to discover the proximity information along with messages from neighborhoods to target nodes.
- We propose a self-supervised learning task to preserve graph connectivity and regularize the augmented graph data to generate the representations.
- Extensive experiments demonstrate that our model outperforms baselines on benchmark datasets and improves degree fairness.
 

## The DegFairGT is available at:
* [![GitHub](https://img.shields.io/badge/GitHub-Data%20&%20Code-9B9B9B?style=flat-square&logo=GitHub)](https://github.com/NSLab-CUK/Community-aware-Graph-Transformer)
* [![arXiv](https://img.shields.io/badge/arXiv-2312.16788-b31b1b?style=flat-square&logo=arxiv&logoColor=red)](https://arxiv.org/abs/2312.16788)

## Cite "DegFairGT" as: 

Please cite our [paper](https://arxiv.org/abs/2504.15075) if you find *DegFairGT* useful in your work:
```
@misc{hoang2025mitigatingdegreebiasgraph,
      title={Mitigating Degree Bias in Graph Representation Learning with Learnable Structural Augmentation and Structural Self-Attention}, 
      author={Van Thuy Hoang and Hyeon-Ju Jeon and O-Joun Lee},
      year={2025},
      eprint={2504.15075},
      archivePrefix={arXiv},
      primaryClass={cs.AI},
      url={https://arxiv.org/abs/2504.15075}, 
}
```

:page_facing_up::woman_technologist::bookmark_tabs::label::black_nib:	

## Contributors: 

<a href="https://github.com/NSLab-CUK/Unified-Graph-Transformer/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=NSLab-CUK/Unified-Graph-Transformer" />
</a>

***

<a href="https://nslab-cuk.github.io/"><img src="https://github.com/NSLab-CUK/NSLab-CUK/raw/main/Logo_Dual_Wide.png"/></a>

***

