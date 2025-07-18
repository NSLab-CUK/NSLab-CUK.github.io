---
layout: page
title: Graph Learning Reading List for Newcomers
permalink: /research/reading-list-for-newcomers/2023-12-14/
image: Bib_Network.png
description: This reading list is designed to help newcomers to the Network Science Lab @ CUK understand the fundamental concepts and models in graph learning.
toc: true
toc_sticky: true
toc_label: "Table of Contents"
---

<!-- ![image](https://github.com/NSLab-CUK/NSLab-CUK.github.io/assets/100113405/96ea07b1-9117-4436-9e78-5f554d6629a4) -->

This reading list is designed to help newcomers to the Network Science Lab @ CUK understand the fundamental concepts and models in graph learning.

_Last updated: Dec 14th, 2023_

***

## Shallow Graph Models
- **DeepWalk**: Perozzi, B., Al-Rfou, R., Skiena, S. (2014). **DeepWalk: Online Learning of Social Representations.** *Proceedings of the 20th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD 2014)*, 701–710.
- **node2vec**: Grover, A., Leskovec, J. (2016). **node2vec: Scalable Feature Learning for Networks.** *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD 2016)*, 855–864.
- **LINE**: Tang, J., Qu, M., Wang, M., Zhang, M., Yan, J., Mei, Q. (2015). **LINE: Large-scale Information Network Embedding.** *Proceedings of the 24th International Conference on World Wide Web (WWW 2015)*, 1067–1077.
- **Asymmetric Transitivity**: Ou, M., Cui, P., Pei, J., Zhang, Z., Zhu, W. (2016). **Asymmetric Transitivity Preserving Graph Embedding.** *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD 2016)*, 1105–1114.
- **SDNE**: Wang, D., Cui, P., Zhu, W. (2016). **Structural Deep Network Embedding.** *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD 2016)*, 1225–1234.
- **GraRep**: Cao, S., Lu, W., Xu, Q. (2015). **GraRep: Learning Graph Representations with Global Structural Information.** *Proceedings of the 24th ACM International Conference on Information and Knowledge Management (CIKM 2015)*, 891–900.
- **SkipWalk**: Perozzi, B., Kulkarni, V., Chen, H., Skiena, S. (2017). **Don't Walk, Skip!: Online Learning of Multi-scale Network Embeddings.** *Proceedings of the 2017 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining (ASONAM 2017)*, 258–265.
- **struc2vec**: Ribeiro, L. F. R., Saverese, P. H. P., Figueiredo, D. R. (2017). **struc2vec: Learning Node Representations from Structural Identity.** *Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD 2017)*, 385–394.
- **subgraph2vec**: Narayanan, A., Chandramohan, M., Chen, L., Liu, Y., Saminathan, S. (2016). **subgraph2vec: Learning Distributed Representations of Rooted Sub-graphs from Large Graphs.** arXiv:1606.08928.
- **metapath2vec**: Dong, Y., Chawla, N. V., Swami, A. (2017). **metapath2vec: Scalable Representation Learning for Heterogeneous Networks.** *Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD 2017)*, 135–144.
- **Deep Gaussian Embedding**: Bojchevski, A., Günnemann, S. (2018). **Deep Gaussian Embedding of Graphs: Unsupervised Inductive Learning via Ranking.** *International Conference on Learning Representations (ICLR 2018)*.

## Deep Graph Models

### Recurrent GNNs
- Li, Y., Tarlow, D., Brockschmidt, M., Zemel, R. (2015). **Gated Graph Sequence Neural Networks.** arXiv:1511.05493.
- Gilmer, J., Schoenholz, S. S., Riley, P. F., Vinyals, O., Dahl, G. E. (2017). **Neural Message Passing for Quantum Chemistry.** *Proceedings of the 34th International Conference on Machine Learning (ICML 2017)*, 1263–1272.

### Graph Autoencoders
- Wang, D., Cui, P., Zhu, W. (2016). **Structural Deep Network Embedding.** *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD 2016)*, 1225–1234.
- Tu, K., Cui, P., Wang, X., Wang, F., Zhu, W. (2018). **Structural Deep Embedding for Hyper-Networks.** *Proceedings of the 32nd AAAI Conference on Artificial Intelligence (AAAI 2018)*, 426–433.

### Spatial GNNs
- Hamilton, W. L., Ying, Z., Leskovec, J. (2017). **Inductive Representation Learning on Large Graphs.** *Proceedings of the 31st Conference on Neural Information Processing Systems (NeurIPS 2017)*, 1024–1034.
- Chen, J., Ma, T., Xiao, C. (2018). **FastGCN: Fast Learning with Graph Convolutional Networks via Importance Sampling.** *International Conference on Learning Representations (ICLR 2018)*.
- Chiang, W., Liu, X., Si, S., Li, Y., Bengio, S., Hsieh, C. (2019). **Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph Convolutional Networks.** *Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD 2019)*, 257–266.
- Li, G., Xiong, C., Thabet, A. K., Ghanem, B. (2020). **DeeperGCN: All You Need to Train Deeper GCNs.** arXiv:2006.07739.
- Chen, M., Wei, Z., Huang, Z., Ding, B., Li, Y. (2020). **Simple and Deep Graph Convolutional Networks.** *Proceedings of the 37th International Conference on Machine Learning (ICML 2020)*, 1725–1735.

### Attentive GNNs
- Velickovic, P., Cucurull, G., Casanova, A., Romero, A., Liò, P., Bengio, Y. (2017). **Graph Attention Networks.** arXiv:1710.10903.
- Ye, Y., Ji, S. (2023). **Sparse Graph Attention Networks.** *IEEE Transactions on Knowledge and Data Engineering (TKDE)*, 35(1), 905–916.
- Li, H., Huang, S. H., Ye, T., Xiuyan, G. (2019). **Graph Star Net for Generalized Multi-Task Learning.** arXiv:1906.12330.
- Kim, D., Oh, A. (2021). **How to Find Your Friendly Neighborhood: Graph Attention Design with Self-Supervision.** *International Conference on Learning Representations (ICLR 2021)*.
- Wang, G., Ying, R., Huang, J., Leskovec, J. (2019). **Improving Graph Attention Networks with Large Margin-Based Constraints.** arXiv:1910.11945.

### Limitations of GNNs and Their Solutions
- Morris, C., Ritzert, M., Fey, M., Hamilton, W. L., Lenssen, J. E., Rattan, G., Grohe, M. (2019). **Weisfeiler and Leman Go Neural: Higher-Order Graph Neural Networks.** *Proceedings of the 33rd AAAI Conference on Artificial Intelligence (AAAI 2019)*, 4602–4609.
- Yu, H., Yuan, J., Yao, Y., Wang, C. (2022). **Not All Edges Are Peers: Accurate Structure-Aware Graph Pooling Networks.** *Neural Networks*, 156, 58–66.
- Shu, J., Xi, B., Li, Y., Wu, F., Kamhoua, C. A., Ma, J. (2022). **Understanding Dropout for Graph Neural Networks.** *Proceedings of the Companion Volume of The Web Conference (WWW 2022)*, 1128–1138.

### Transformers with GNNs
- Shi, Y., Huang, Z., Feng, S., Zhong, H., Wang, W., Sun, Y. (2021). **Masked Label Prediction: Unified Message Passing Model for Semi-Supervised Classification.** *Proceedings of the Thirtieth International Joint Conference on Artificial Intelligence (IJCAI 2021)*, 1548–1554.
- Nguyen, D. Q., Nguyen, T. D., Phung, D. (2022). **Universal Graph Transformer Self-Attention Networks.** *Proceedings of The Web Conference 2022 (WWW 2022)*, 193–196.

### Structure-Aware Graph Transformers
- Chen, D., O'Bray, L., Borgwardt, K. M. (2022). **Structure-Aware Transformer for Graph Representation Learning.** *Proceedings of the 39th International Conference on Machine Learning (ICML 2022)*, 3469–3489.
- Kim, J., Nguyen, T. D., Min, S., Cho, S., Lee, M., Lee, H., Hong, S. (2022). **Pure Transformers Are Powerful Graph Learners.** arXiv:2207.02505.
- Ying, C., Cai, T., Luo, S., Zheng, S., Ke, G., He, D., Shen, Y., Liu, T. Y. (2021). **Do Transformers Really Perform Badly for Graph Representation?** *Proceedings of the 35th Conference on Neural Information Processing Systems (NeurIPS 2021)*, 28877–28888.
- Dwivedi, V. P., Luu, A. T., Laurent, T., Bengio, Y., Bresson, X. (2022). **Graph Neural Networks with Learnable Structural and Positional Representations.** *International Conference on Learning Representations (ICLR 2022)*.
- Hussain, M. S., Zaki, M. J., Subramanian, D. (2022). **Global Self-Attention as a Replacement for Graph Convolution.** *Proceedings of the 28th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD 2022)*, 655–665.
- Zhao, H., Ma, S., Zhang, D., Deng, Z. H., Wei, F. (2023). **Are More Layers Beneficial to Graph Transformers?** *International Conference on Learning Representations (ICLR 2023)*.
- Ma, L., Lin, C., Lim, D., Romero-Soriano, A., Dokania, P. K., Coates, M., Torr, P. H. S., Lim, S. N. (2023). **Graph Inductive Biases in Transformers without Message Passing.** *Proceedings of the 40th International Conference on Machine Learning (ICML 2023)*, 23321–23337.
- Ma, X., Chen, Q., Wu, Y., Song, G., Wang, L., Zheng, B. (2023). **Rethinking Structural Encodings: Adaptive Graph Transformer for Node Classification Task.** *Proceedings of The Web Conference 2023 (WWW 2023)*, 533–544.
- Mao, Q., Liu, Z., Liu, C., Sun, J. (2023). **HINormer: Representation Learning on Heterogeneous Information Networks with Graph Transformer.** *Proceedings of The Web Conference 2023 (WWW 2023)*, 599–610.
- Mialon, G., Chen, D., Selosse, M., Mairal, J. (2021). **GraphiT: Encoding Graph Structure in Transformers.** arXiv:2106.05667.
- Wu, Z., Jain, P., Wright, M. A., Mirhoseini, A., Gonzalez, J. E., Stoica, I. (2021). **Representing Long-Range Context for Graph Neural Networks with Global Attention.** *Proceedings of the 35th Conference on Neural Information Processing Systems (NeurIPS 2021)*, 13266–13279.
- Rampásek, L., Galkin, M., Dwivedi, V. P., Luu, A. T., Wolf, G., Beaini, D. (2022). **Recipe for a General, Powerful, Scalable Graph Transformer.** *Proceedings of the 36th Conference on Neural Information Processing Systems (NeurIPS 2022)*.
- Shirzad, H., Velingker, A., Venkatachalam, B., Sutherland, D. J., Sinop, A. K. (2023). **Exphormer: Sparse Transformers for Graphs.** *Proceedings of the 40th International Conference on Machine Learning (ICML 2023)*, 31613–31632.

### Graph Transformer and Sampling Strategies
- Zhao, J., Li, C., Wen, Q., Wang, Y., Liu, Y., Sun, H., Xie, X., Ye, Y. (2022). **Gophormer: Ego-Graph Transformer for Node Classification.** *Proceedings of the 36th Conference on Neural Information Processing Systems (NeurIPS 2022)*.
- Coarformer Team (2021). **Coarformer: Transformer for Large Graphs via Graph Coarsening.** *OpenReview (2021)*.
- Zhang, Z., Liu, Q., Hu, Q., Lee, C. K. (2022). **Hierarchical Graph Transformer with Adaptive Node Sampling.** *Proceedings of the 36th Conference on Neural Information Processing Systems (NeurIPS 2022)*.
- Chen, J., Gao, K., Li, G., He, K. (2023). **NAGphormer: A Tokenized Graph Transformer for Node Classification in Large Graphs.** *International Conference on Learning Representations (ICLR 2023)*.
