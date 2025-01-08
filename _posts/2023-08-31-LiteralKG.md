---
layout: post
title: LiteralKG, A Novel GNN Model for Learning Literal-aware Representations of Medical Knowledge Graphs
date:   2023-08-31 00:00:00 +0900
tags:   Release
image:  Bib_Network.png
published: true
description: The Network Science Lab at the Catholic University of Korea releases LiteralKG, a novel GNN model for learning literal-aware representations of medical knowledge graphs to integrate literal information and graph structural features into unified vector representations.
---

We present [LiteralKG](https://github.com/NSLab-CUK/LiteralKG), a novel GNN model for learning literal-aware representations of medical knowledge graphs, which can integrate different types of literal information and graph structural features into unified vector representations. LiteralKG is developed by NS Lab, CUK, based on pure PyTorch backend.

<p align="center">
  <img src="/images/LiteralKG.jpg" alt="LiteralKG Architecture" width="800">
  <br>
  <b></b> The overall architecture of LiteralKG.
</p>

Over the past few years, Knowledge Graph (KG) embedding has been used to benefit the diagnosis of animal diseases by analyzing electronic medical records (EMRs), such as notes and veterinary records. However, learning representations to capture entities and relations with literal information in KGs is challenging as the KGs show heterogeneous properties and various types of literal information. Meanwhile, the existing methods mostly aim to preserve graph structures surrounding target nodes without considering different types of literals, which could also carry significant information. We propose **LiteralKG**, a knowledge graph embedding model for efficiently diagnosing animal diseases, which could learn various types of literal information and graph structure and fuse them into unified representations. Specifically, we construct a knowledge graph that is built from EMRs along with literal information collected from various animal hospitals. We then fuse different types of entities and node feature information into unified vector representations through gate networks. Finally, we propose a self-supervised learning task to learn graph structure in pretext tasks and then towards various downstream tasks. Experimental results on link prediction tasks demonstrate that our model outperforms the baselines that consist of state-of-the-art models.

## A short description of **LiteralKG**:

- We construct a medical knowledge graph that comprises 595,172 entities and 16 relation types from various EMRs.
- **LiteralKG** could learn different types of literal information and graph structure and then fuse them into unified representations.
- **LiteralKG**, a self-supervised learning framework for Knowledge Graph, that could learn the graph structure from pretext tasks to generate representations, and then the pre-trained model is used for downstream tasks to predict animal diseases.
- The experimental results on the KG with different types of GNN aggregators and residual connection and identity mapping show the superiority of **LiteralKG** over baselines.

## The **LiteralKG** is available at:
* [![GitHub](https://img.shields.io/badge/GitHub-Data%20&%20Code-9B9B9B?style=flat-square&logo=GitHub)](https://github.com/NSLab-CUK/LiteralKG)
* [![DOI](http://img.shields.io/:DOI-10.1109/ACCESS.2023.3324046-FAB70C?style=flat-square&logo=doi)](https://doi.org/10.1109/ACCESS.2023.3324046)
* [![arXiv](https://img.shields.io/badge/arXiv-2309.03219-b31b1b?style=flat-square&logo=arxiv&logoColor=red)](https://arxiv.org/abs/2309.03219)
* [![PWC](https://custom-icon-badges.demolab.com/badge/Papers%20With%20Code-LiteralKG-21CBCE?style=flat-square&logo=paperswithcode)](https://paperswithcode.com/paper/companion-animal-disease-diagnostics-based-on)


## Cite "**LiteralKG**" as:

Please cite our [paper](https://ieeexplore.ieee.org/abstract/document/10283810) if you find *LiteralKG* useful in your work:
```
@Article{Hoang2023,
  author  = {Van Thuy Hoang and Thanh Sang Nguyen and Sangmyeong Lee and Jooho Lee and Luong Vuong Nguyen and O-Joun Lee},
  title   = {Companion Animal Disease Diagnostics Based on Literal-Aware Medical Knowledge Graph Representation Learning},
  journal = {IEEE Access},
  year    = {2023},
  volume  = {11},
  pages   = {114238--114249},
  month   = oct,
  issn    = {2169-3536},
  doi     = {10.1109/ACCESS.2023.3324046},
}
```

:page_facing_up::woman_technologist::bookmark_tabs::label::black_nib:	

## Contributors: 

<a href="https://github.com/NSLab-CUK/LiteralKG/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=NSLab-CUK/LiteralKG" />
</a>

***

<a href="https://nslab-cuk.github.io/"><img src="https://github.com/NSLab-CUK/NSLab-CUK/raw/main/Logo_Dual_Wide.png"/></a>

***

