---
layout: page
title: Graph Learning Reading List for Newcomers
permalink: /research/reading-list-for-newcomers/
image: Bib_Network.png
description: This reading list is designed to help newcomers to the Network Science Lab @ CUK understand the fundamental concepts and models in graph learning.
toc: true
toc_sticky: true
toc_label: "Table of Contents"
---

<!-- ![image](https://github.com/NSLab-CUK/NSLab-CUK.github.io/assets/100113405/96ea07b1-9117-4436-9e78-5f554d6629a4) -->

This reading list is designed to help newcomers to the Network Science Lab @ CUK understand the fundamental concepts and models in graph learning.

_Last updated: Jul 18th, 2025_

***

<h5>Previous Versions</h5>
{:.no_toc}

* [Dec 14th, 2023](https://nslab-cuk.github.io/research/reading-list-for-newcomers/2023-12-14/)

***

## Shallow Graph Models

* **Perozzi, B., Al-Rfou, R., & Skiena, S. (2014).** DeepWalk: Online Learning of Social Representations. In *Proceedings of the 20th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining* (pp. 701–710). doi:10.1145/2623330.2623732
* **Grover, A., & Leskovec, J. (2016).** node2vec: Scalable Feature Learning for Networks. In *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining* (pp. 855–864). doi:10.1145/2939672.2939754
* **Tang, J., Qu, M., Wang, M., Zhang, M., Yan, J., & Mei, Q. (2015).** LINE: Large-scale Information Network Embedding. In *Proceedings of the 24th International Conference on World Wide Web (WWW ’15)* (pp. 1067–1077). doi:10.1145/2736277.2741093
* **Ou, M., Cui, P., Pei, J., Zhang, Z., & Zhu, W. (2016).** Asymmetric Transitivity Preserving Graph Embedding. In *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining* (pp. 1105–1114). doi:10.1145/2939672.2939756
* **Cao, S., Lu, W., & Xu, Q. (2015).** GraRep: Learning Graph Representations with Global Structural Information. In *Proceedings of the 24th ACM International on Conference on Information and Knowledge Management (CIKM ’15)* (pp. 891–900). doi:10.1145/2806416.2806462
* **Perozzi, B., Kulkarni, V., Chen, H., & Skiena, S. (2017).** Don’t Walk, Skip!: Online Learning of Multi-scale Network Embeddings. In *Proceedings of the 2017 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining (ASONAM ’17)* (pp. 258–265). doi:10.1109/ASONAM.2017.82
* **Ribeiro, L. F., Saverese, P. H. P., & Figueiredo, D. R. (2017).** struc2vec: Learning Node Representations from Structural Identity. In *Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD ’17)* (pp. 385–394). doi:10.1145/3097983.3098036
* **Narayanan, A., Chandramohan, M., Chen, L., Liu, Y., & Saminathan, S. (2016).** subgraph2vec: Learning Distributed Representations of Rooted Sub-graphs from Large Graphs. *CoRR*, abs/1606.08928.
* **Dong, Y., Chawla, N. V., & Swami, A. (2017).** metapath2vec: Scalable Representation Learning for Heterogeneous Networks. In *Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD ’17)* (pp. 135–144). doi:10.1145/3097983.3098036
* **Bojchevski, A., & Günnemann, S. (2018).** Deep Gaussian Embedding of Graphs: Unsupervised Inductive Learning via Ranking. In *International Conference on Learning Representations (ICLR ’18)*.

***

## Deep Graph Models

### Graph Autoencoders

* **Kipf, T. N., & Welling, M. (2016).** Variational Graph Auto-Encoders. *arXiv:1611.07308*
* **Wang, D., Cui, P., & Zhu, W. (2016).** Structural Deep Network Embedding (SDNE). In *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining* (pp. 1225–1234). doi:10.1145/2939672.2939753
* **Tu, K., Cui, P., Wang, X., Wang, F., & Zhu, W. (2018).** Structural Deep Embedding for Hyper-Networks. In *AAAI 2018* (pp. 426–433).

### Spatial GNNs

* **Kipf, T. N., & Welling, M. (2017).** Semi-Supervised Classification with Graph Convolutional Networks. *ICLR 2017*.
* **Hamilton, W. L., Ying, Z., & Leskovec, J. (2017).** Inductive Representation Learning on Large Graphs (GraphSAGE). *NeurIPS 2017*, 1024–1034.
* **Chen, J., Ma, T., & Xiao, C. (2018).** FastGCN: Fast Learning with Graph Convolutional Networks via Importance Sampling. *ICLR 2018*.
* **Chiang, W., Liu, X., Si, S., Li, Y., Bengio, S., & Hsieh, C.-J. (2019).** Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph Convolutional Networks. *KDD 2019*, 257–266.
* **Li, G., Xiong, C., Thabet, A. K., & Ghanem, B. (2020).** DeeperGCN: All You Need to Train Deeper GCNs. *arXiv:2006.07739*.
* **Chen, M., Wei, Z., Huang, Z., Ding, B., & Li, Y. (2020).** Simple and Deep Graph Convolutional Networks. *ICML 2020*, Vol. 119, 1725–1735.
* **Xu, K., Hu, W., Leskovec, J., & Jegelka, S. (2018).** How Powerful Are Graph Neural Networks? *ICLR 2019*.

### Attentive GNNs

* **Veličković, P., Cucurull, G., Casanova, A., Romero, A., Liò, P., & Bengio, Y. (2018).** Graph Attention Networks. *ICLR 2018*.
* **Hong, X., Li, W., Wang, C., Lin, M., & Lu, S. (2024).** Label Attentive Distillation for GNN-Based Graph Classification. *AAAI 2024*, 8499–8507.
* **Ye, Y., & Ji, S. (2023).** Sparse Graph Attention Networks. *IEEE Trans. Knowl. Data Eng.*, 35(1), 905–916.
* **Kim, D., & Oh, A. (2021).** How to Find Your Friendly Neighborhood: Graph Attention Design with Self-Supervision. *ICLR 2021*.
* **Brody, S., Alon, U., & Yahav, E. (2022).** How Attentive Are Graph Attention Networks? *ICLR 2022*.

***

## Limitations of GNNs and Their Solutions

### GNNs with Scalability

* **Chen, J., Ma, T., & Xiao, C. (2018).** FastGCN: Fast Learning with Graph Convolutional Networks via Importance Sampling. In *Proceedings of the 6th International Conference on Learning Representations (ICLR ’18)*. OpenReview\.net.
* **Chiang, W., Liu, X., Si, S., Li, Y., Bengio, S., & Hsieh, C.-J. (2019).** Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph Convolutional Networks. In *Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining* (pp. 257–266). ACM.
* **Li, G., Xiong, C., Thabet, A. K., & Ghanem, B. (2020).** DeeperGCN: All You Need to Train Deeper GCNs. *CoRR*, abs/2006.07739.
* **Chen, M., Wei, Z., Huang, Z., Ding, B., & Li, Y. (2020).** Simple and Deep Graph Convolutional Networks. In *Proceedings of the 37th International Conference on Machine Learning (ICML ’20)* (Vol. 119, pp. 1725–1735). PMLR.
* **Kong, K., Chen, J., Kirchenbauer, J., Ni, R., Bruss, C. B., & Goldstein, T. (2023).** GOAT: A Global Transformer on Large-scale Graphs. In *Proceedings of the 40th International Conference on Machine Learning (ICML ’23)* (pp. 17375–17390). PMLR.
* **Liu, C., Zhan, Y., Ma, X., Ding, L., Tao, D., Wu, J., & Hu, W. (2023).** Gapformer: Graph Transformer with Graph Pooling for Node Classification. In *Proceedings of the 32nd International Joint Conference on Artificial Intelligence (IJCAI ’23)* (pp. 2196–2205). IJCAI.
* **Chen, J., Gao, K., Li, G., & He, K. (2023).** NAGphormer: A Tokenized Graph Transformer for Node Classification in Large Graphs. In *Proceedings of the International Conference on Learning Representations (ICLR ’23)*. OpenReview\.net.

### GNNs with Fairness

* **Jiang, Z., Han, X., Fan, C., Liu, Z., Zou, N., Mostafavi, A., & Hu, X. (2024).** Chasing Fairness in Graphs: A GNN Architecture Perspective. *Proceedings of the AAAI Conference on Artificial Intelligence, 38*(19), 21214–21222.
* **Wang, R., Wang, X., Shi, C., & Song, L. (2022).** Uncovering the Structural Fairness in Graph Contrastive Learning. In *Advances in Neural Information Processing Systems* (NeurIPS 2022), 35, 32465–32473.
* **Liu, Z., Nguyen, T.-K., & Fang, Y. (2023).** On Generalized Degree Fairness in Graph Neural Networks. *Proceedings of the AAAI Conference on Artificial Intelligence, 37*(4), 4525–4533.
* **Pan, C., Yang, C., Gong, Z., Qin, C., Xu, J., Liu, Z., & Tong, H. (2024).** Towards Fair Graph Federated Learning via Incentive Mechanisms. *Proceedings of the AAAI Conference on Artificial Intelligence, 38*(13).
* **Luo, R., Huang, H., Yu, S., Zhang, X., & Xia, F. (2024).** FairGT: A Fairness-Aware Graph Transformer. In *Proceedings of the Thirty-Third International Joint Conference on Artificial Intelligence (IJCAI 2024)* (pp. 50–57).
* **Liu, Z., Qiu, R., Zeng, Z., Yoo, H., Zhou, D., Xu, Z., & Tong, H. (2024).** Class-Imbalanced Graph Learning without Class Rebalancing. *International Conference on Learning Representations (ICLR 2024)*.

### GNNs with Heterophily

* **Wang, J., Guo, Y., Yang, L., & Wang, Y. (2024).** Understanding heterophily for graph neural networks. In *Proceedings of the 41st International Conference on Machine Learning (ICML 2024)* (Vol. 235, pp. 50489–50529). PMLR.
* **Park, M., Heo, J., & Kim, D. (2024).** Mitigating oversmoothing through reverse process of GNNs for heterophilic graphs. *arXiv* preprint arXiv:2403.10543.
* **Wu, Y., Yao, J., Han, B., Yao, L., & Liu, T. (2024).** Unraveling the impact of heterophilic structures on graph positive-unlabeled learning. *arXiv* preprint arXiv:2405.19919.
* **Luan, S., Hua, C., Lu, Q., Zhu, J., Zhao, M., Zhang, S., Chang, X.-W., & Precup, D. (2022).** Revisiting heterophily for graph neural networks. In *Advances in Neural Information Processing Systems (NeurIPS 2022)* (Vol. 35, pp. 1362–1375).
* **Zhu, J., Rossi, R. A., Rao, A., Mai, T., Lipka, N., Ahmed, N. K., & Koutra, D. (2021).** Graph neural networks with heterophily. In *Proceedings of the AAAI Conference on Artificial Intelligence* (Vol. 35, No. 12, pp. 11168–11176).

### Long-Range Dependency Problems

* **Bamberger, J., Gutteridge, B., Roux, S. L., Bronstein, M. M., & Dong, X. (2025).** On Measuring Long-Range Interactions in Graph Neural Networks. *arXiv preprint*, arXiv:2506.05971.
* **Suresh, S., Budde, V., Neville, J., Li, P., & Ma, J. (2021).** Breaking the Limit of Graph Neural Networks by Improving the Assortativity of Graphs with Local Mixing Patterns. In *Proceedings of the 27th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining* (pp. 1541–1551). ACM.
* **Wu, Z., Jain, P., Wright, M. A., Mirhoseini, A., Gonzalez, J. E., & Stoica, I. (2021).** Representing Long-Range Context for Graph Neural Networks with Global Attention. In *Advances in Neural Information Processing Systems* (Vol. 34, pp. 13266–13279).
* **Chen, D., Schulz, T. H., & Borgwardt, K. (2025).** Learning Long Range Dependencies on Graphs via Random Walks. In *International Conference on Learning Representations (ICLR 2025)*.

### Over-smoothing Problems

* **Park, M., Choi, S., Heo, J., Park, E., & Kim, D. (2025).** The Oversmoothing Fallacy: A Misguided Narrative in GNN Research. *arXiv preprint*, arXiv:2506.04653v1 \[cs.LG], June 5, 2025.
* **Shu, J., Xi, B., Li, Y., Wu, F., Kamhoua, C. A., & Ma, J. (2022).** Understanding Dropout for Graph Neural Networks. In *Companion Proceedings of The Web Conference 2022* (WWW ’22, pp. 1128–1138). ACM.
* **Chen, D., Lin, Y., Li, W., Li, P., Zhou, J., & Sun, X. (2020).** Measuring and Relieving the Over-Smoothing Problem for Graph Neural Networks from the Topological View. In *Proceedings of the AAAI Conference on Artificial Intelligence* (Vol. 34, No. 04, pp. 3438–3445). AAAI Press.
* **Keriven, N. (2022).** Not Too Little, Not Too Much: A Theoretical Analysis of Graph (Over)Smoothing. In *Advances in Neural Information Processing Systems* (NeurIPS ’22, Vol. 35, pp. 2268–2281).
* **Liu, M., Gao, H., & Ji, S. (2020).** Towards Deeper Graph Neural Networks. In *Proceedings of the 26th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining* (KDD ’20, pp. 338–348). ACM.
* **Zhou, K., Huang, X., Li, Y., Zha, D., Chen, R., & Hu, X. (2020).** Towards Deeper Graph Neural Networks with Differentiable Group Normalization. In *Advances in Neural Information Processing Systems* (NeurIPS ’20, Vol. 33).

### Over-squarshing Problems

* **Giraldo, J. H., Malliaros, F. D., et al. (2023).** On the Trade‐off between Over‐smoothing and Over‐squashing in Deep Graph Neural Networks. In *Proceedings of the 32nd ACM International Conference on Information and Knowledge Management (CIKM ’23)*. arXiv:2212.02374
* **Ying, Z., You, J., Morris, C., Ren, X., Hamilton, W., & Leskovec, J. (2018).** Hierarchical Graph Representation Learning with Differentiable Pooling. In *Advances in Neural Information Processing Systems* 31.
* **Sanders, C., Roth, A., & Liebig, T. (2023).** Curvature‐Based Pooling within Graph Neural Networks. *arXiv preprint*, arXiv:2308.16516.
* **Liu, Y., Zhou, C., Pan, S., Wu, J., Li, Z., Chen, H., & Zhang, P. (2023).** CurvDrop: A Ricci Curvature‐Based Approach to Prevent Graph Neural Networks from Over‐Smoothing and Over‐Squashing. In *The Web Conference (WWW ’23)* (pp. 221–230).
* **Di Giovanni, F., Giusti, L., Barbero, F., Luise, G., Liò, P., & Bronstein, M. (2023).** On Over‐Squashing in Message Passing Neural Networks: The Impact of Width, Depth, and Topology. In *International Conference on Machine Learning (ICML ’23)*. arXiv:2302.02941
* **Alon, U., & Yahav, E. (2021).** On the Bottleneck of Graph Neural Networks and Its Practical Implications. In *International Conference on Learning Representations (ICLR ’21)*. arXiv:2006.05205

### Over-globalizing Problems

* **Xing, Y., Wang, X., Li, Y., Huang, H., & Shi, C. (2024).** Less Is More: On the Over-Globalizing Problem in Graph Transformers. *arXiv preprint*, arXiv:2405.01102.
* **Yadati, N. (2025).** LocalFormer: Mitigating Over-Globalising in Transformers on Graphs with Localised Training. *Transactions on Machine Learning Research*, 2025.
* **Wu, Q., Zhao, W., Yang, C., Zhang, H., Nie, F., Jiang, H., Bian, Y., & Yan, J. (2023).** SGFormer: Simplifying and Empowering Transformers for Large-Graph Representations. In *Advances in Neural Information Processing Systems* (NeurIPS 2023).

***

## Graph Transformers

### GNNs with Graph Transformers

- Shi, Y.; Huang, Z.; Feng, S.; Zhong, H.; Wang, W.; Sun, Y. Masked Label Prediction: Unified Message Passing Model for Semi-Supervised Classification. In Proceedings of the Proceedings of the Thirtieth International Joint Conference on Artificial Intelligence (IJCAI 2021). 
- Nguyen, D.Q.; Nguyen, T.D.; Phung, D. Universal Graph Transformer Self-Attention Networks. In Proceedings of the Companion Proceedings of the Web Conference 2022. WWW ’22 
- Yu Rong, Yatao Bian, Tingyang Xu, Weiyang Xie, Ying Wei, Wenbing Huang, Junzhou Huang: Self-Supervised Graph Transformer on Large-Scale Molecular Data. NeurIPS 2020

### Structure-aware Graph Transformers

- Van Thuy Hoang, O-Joun Lee: Transitivity-Preserving Graph Representation Learning for Bridging Local Connectivity and Role-Based Similarity. AAAI 2024
- Dexiong Chen, Leslie O'Bray, Karsten M. Borgwardt: Structure-Aware Transformer for Graph Representation Learning. ICML 2022 
- Jinwoo Kim, Tien Dat Nguyen, Seonwoo Min, Sungjun Cho, Moontae Lee, Honglak Lee, Seunghoon Hong: Pure Transformers are Powerful Graph Learners. ArXiv 2022
- Chengxuan Ying, Tianle Cai, Shengjie Luo, Shuxin Zheng, Guolin Ke, Di He, Yanming Shen, Tie-Yan Liu: Do Transformers Really Perform Badly for Graph Representation? NeurIPS 2021.
- Vijay Prakash Dwivedi, Anh Tuan Luu, Thomas Laurent, Yoshua Bengio, Xavier Bresson: Graph Neural Networks with Learnable Structural and Positional Representations. ICLR 2022
- Md. Shamim Hussain, Mohammed J. Zaki, Dharmashankar Subramanian: Global Self-Attention as a Replacement for Graph Convolution. KDD 2022: 655-665
- Haiteng Zhao, Shuming Ma, Dongdong Zhang, Zhi-Hong Deng, Furu Wei: Are More Layers Beneficial to Graph Transformers? ICLR 2023
- Liheng Ma, Chen Lin, Derek Lim, Adriana Romero-Soriano, Puneet K. Dokania, Mark Coates, Philip H. S. Torr, Ser-Nam Lim: Graph Inductive Biases in Transformers without Message Passing. ICML 2023
- Xiaojun Ma, Qin Chen, Yi Wu, Guojie Song, Liang Wang, Bo Zheng: Rethinking Structural Encodings: Adaptive Graph Transformer for Node Classification Task. WWW 2023: 533-544
- Qiheng Mao, Zemin Liu, Chenghao Liu, Jianling Sun: HINormer: Representation Learning On Heterogeneous Information Networks with Graph Transformer. WWW 2023: 599-610
- Zhanghao Wu, Paras Jain, Matthew A. Wright, Azalia Mirhoseini, Joseph E. Gonzalez, Ion Stoica: Representing Long-Range Context for Graph Neural Networks with Global Attention. NeurIPS 2021: 13266-13279
- Ladislav Rampásek, Michael Galkin, Vijay Prakash Dwivedi, Anh Tuan Luu, Guy Wolf, Dominique Beaini: Recipe for a General, Powerful, Scalable Graph Transformer. NeurIPS 2022
- Hamed Shirzad, Ameya Velingker, Balaji Venkatachalam, Danica J. Sutherland, Ali Kemal Sinop: Exphormer: Sparse Transformers for Graphs. ICML 2023: 31613-31632

### Graph Transformers and Sampling Strategies

- Jianan Zhao, Chaozhuo Li, Qianlong Wen, Yiqi Wang, Yuming Liu, Hao Sun, Xing Xie, Yanfang Ye: Gophormer: Ego-Graph Transformer for Node Classification
- Kuang, Weirui, et al. Coarformer: Transformer for large graph via graph coarsening. Openreview 2021.
- Zaixi Zhang, Qi Liu, Qingyong Hu, Chee-Kong Lee: Hierarchical Graph Transformer with Adaptive Node Sampling. NeurIPS 2022
- Jinsong Chen, Kaiyuan Gao, Gaichao Li, Kun He: NAGphormer: A Tokenized Graph Transformer for Node Classification in Large Graphs. ICLR 2023
- Grégoire Mialon, Dexiong Chen, Margot Selosse, Julien Mairal: GraphiT: Encoding Graph Structure in Transformers. CoRR abs/2106.05667 (2021).

***

## Advanced Graph Neural Networks

### Pre-training Graph Neural Networks

- Weihua Hu, Bowen Liu, Joseph Gomes, Marinka Zitnik, Percy Liang, Vijay S. Pande, Jure Leskovec: Strategies for Pre-training Graph Neural Networks. ICLR 2020
- Yuning You, Tianlong Chen, Yang Shen, Zhangyang Wang: Graph Contrastive Learning Automated. ICML 2021: 12121-12132
- Yuning You, Tianlong Chen, Yongduo Sui, Ting Chen, Zhangyang Wang, Yang Shen: Graph Contrastive Learning with Augmentations. NeurIPS 2020
- Minghao Xu, Hang Wang, Bingbing Ni, Hongyu Guo, Jian Tang: Self-supervised Graph-level Representation Learning with Local and Global Structure. ICML 2021: 11548-11558
- Arjun Subramonian: MOTIF-Driven Contrastive Learning of Graph Representations. AAAI 2021
- Zaixi Zhang, Qi Liu, Hao Wang, Chengqiang Lu, Chee-Kong Lee: Motif-based Graph Self-Supervised Learning for Molecular Property Prediction. NeurIPS 2021 
- Kha-Dinh Luong, Ambuj K. Singh: Fragment-based Pretraining and Finetuning on Molecular Graphs. NeurIPS 2023
- Yu Rong, Yatao Bian, Tingyang Xu, Weiyang Xie, Ying Wei, Wenbing Huang, Junzhou Huang: Self-Supervised Graph Transformer on Large-Scale Molecular Data. NeurIPS 2020
- Zhiyuan Liu, Yaorui Shi, A Zhang, Enzhi Zhang, Kenji Kawaguchi, Xiang Wang, Tat-Seng Chua: Rethinking Tokenizer and Decoder in Masked Graph Modeling for Molecules. NeurIPS 2023
- Eric Inae, Gang Liu, Meng Jiang: Motif-aware Attribute Masking for Molecular Graph Pre-training. CoRR abs/2309.04589 (2023)
- Van Thuy Hoang and O-Joun Lee, Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned Graph Information Bottleneck, AAAI 2025.

### Expressive Graph Neural Networks

- Xu, Keyulu, Weihua Hu, Jure Leskovec, and Stefanie Jegelka. "How powerful are graph neural networks?." arXiv preprint arXiv:1810.00826 (2018).
- Christopher Morris, Martin Ritzert, Matthias Fey, William L. Hamilton, Jan Eric Lenssen, Gaurav Rattan, Martin Grohe: Weisfeiler and Leman Go Neural: Higher-Order Graph Neural Networks. AAAI 2019
- Haggai Maron, Heli Ben-Hamu, Hadar Serviansky, Yaron Lipman: Provably Powerful Graph Networks. NeurIPS 2019
- Cristian Bodnar, Fabrizio Frasca, Nina Otter, Yuguang Wang, Pietro Liò, Guido F. Montúfar, Michael M. Bronstein: Weisfeiler and Lehman Go Cellular: CW Networks. NeurIPS 2021
- Zhengdao Chen, Soledad Villar, Lei Chen, Joan Bruna: On the equivalence between graph isomorphism testing and function approximation with GNNs. NeurIPS 2019
- Tom Wollschläger, Niklas Kemper, Leon Hetzel, Johanna Sommer, Stephan Günnemann: Expressivity and Generalization: Fragment-Biases for Molecular GNNs. ICML 2024
- Zhang, B., Luo, S., Wang, L., & He, D. (2023). Rethinking the expressive power of gnns via graph biconnectivity. ICLR 2023.
- Zhou, C., Wang, X., & Zhang, M. From relational pooling to subgraph gnns: A universal framework for more expressive graph neural networks. ICML 2023.

### Multi-view Graph Neural Networks

- GraphMVP: Shengchao Liu, Hanchen Wang, Weiyang Liu, Joan Lasenby, Hongyu Guo, Jian Tang: Pre-training Molecular Graph Representation with 3D Geometry. ICLR 2022
- Hannes Stärk, Dominique Beaini, Gabriele Corso, Prudencio Tossou, Christian Dallago, Stephan Günnemann, Pietro Lió: 3D Infomax improves GNNs for Molecular Property Prediction. ICML 2022: 20479-20502
- Seojin Kim, Jaehyun Nam, Junsu Kim, Hankook Lee, Sungsoo Ahn, Jinwoo Shin: Holistic Molecular Representation Learning via Multi-view Fragmentation. Trans. Mach. Learn. Res. 2024 (2024)
- Jun Xia, Chengshuai Zhao, Bozhen Hu, Zhangyang Gao, Cheng Tan, Yue Liu, Siyuan Li, Stan Z. Li: Mole-BERT: Rethinking Pre-training Graph Neural Networks for Molecules. ICLR 2023
- Changsheng Li, Kaihang Mao, Shiye Wang, Ye Yuan, Guoren Wang: Self-Supervised Graph Information Bottleneck for Multiview Molecular Embedding Learning. IEEE Trans. Artif. Intell. 5(4): 1554-1562 (2024)
Tsai, Y. H.; Wu, Y.; Salakhutdinov, R.; and Morency, L. 2021. Self-supervised Learning from a Multi-view Perspective. ICLR 2021
- Velickovic, P.; Fedus, W.; Hamilton, W. L.; Lio, P.; Ben- `gio, Y.; and Hjelm, R. D. 2019. Deep Graph Infomax. ICLR 2019

### Explainable Graph Neural Networks

- Phillip E Pope, Soheil Kolouri, Mohammad Rostami, Charles E Martin, and Heiko Hoffmann. Explainability methods for graph convolutional neural networks. CVPR 2019.
- Ying-Xin Wu, Xiang Wang, A Zhang, Xiangnan He, and Tat-Seng Chua. Discovering invariant rationales for graph neural networks. ICLR 2022.
- Siqi Miao, Mia Liu, and Pan Li. Interpretable and generalizable graph learning via stochastic attention mechanism. PMLR 2022.
- Wenwen Xia, Mincai Lai, Caihua Shan, Yao Zhang, Xinnan Dai, Xiang Li, and Dongsheng Li. Explaining temporal graph models through an explorer-navigator framework. ICLR 2023.
- Huang, Rundong, Farhad Shirani, and Dongsheng Luo. "Factorized explainer for graph neural networks. AAAI 2024.
- Zhao, Tianxiang, et al. Towards faithful and consistent explanations for graph neural networks. Web Search and Data Mining. 2023.
- Azzolin, Steve, et al. Reconsidering faithfulness in regular, self-explainable and domain invariant GNNs. ICLR 2025.

### Few-shot Learning on Graph Neural Networks

- Zhuang, Xiang, et al. Graph sampling-based meta-learning for molecular property prediction. IJCAI  2023.
- Wang, Liang, et al. Pin-tuning: Parameter-efficient in-context tuning for few-shot molecular property prediction. NeulIPS 2024.
- Wu, Shiguang, Yaqing Wang, and Quanming Yao. Why In-Context Learning Models are Good Few-Shot Learners? ICLR 2025.
- Yao, Quanming, et al. Property-aware relation networks for few-shot molecular property prediction. IEEE Transactions on Pattern Analysis and Machine Intelligence 2024. 


