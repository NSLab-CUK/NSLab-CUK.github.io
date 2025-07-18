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

* [Dec 14th, 2023](https://nslab-cuk.github.io/research/reading-list-for-newcomers/2023-12-14/)

***

## Shallow Graph Models
- Bryan Perozzi, Rami Al-Rfou, Steven Skiena: DeepWalk: online learning of social representations. KDD 2014: 701-710
- Aditya Grover, Jure Leskovec: node2vec: Scalable Feature Learning for Networks. KDD 2016: 855-864
- Jian Tang, Meng Qu, Mingzhe Wang, Ming Zhang, Jun Yan, Qiaozhu Mei: LINE: Large-scale Information Network Embedding. WWW 2015: 1067-1077
- Mingdong Ou, Peng Cui, Jian Pei, Ziwei Zhang, Wenwu Zhu: Asymmetric Transitivity Preserving Graph Embedding. KDD 2016: 1105-1114
- Shaosheng Cao, Wei Lu, Qiongkai Xu: GraRep: Learning Graph Representations with Global Structural Information. CIKM 2015: 891-900
- Bryan Perozzi, Vivek Kulkarni, Haochen Chen, Steven Skiena: Don't Walk, Skip!: Online Learning of Multi-scale Network Embeddings. ASONAM 2017: 258-265
- Leonardo Filipe Rodrigues Ribeiro, Pedro H. P. Saverese, Daniel R. Figueiredo: struc2vec: Learning Node Representations from Structural Identity. KDD 2017: 385-394.
- Annamalai Narayanan, Mahinthan Chandramohan, Lihui Chen, Yang Liu, Santhoshkumar Saminathan: subgraph2vec: Learning Distributed Representations of Rooted Sub-graphs from Large Graphs. CoRR abs/1606.08928 (2016)
- Yuxiao Dong, Nitesh V. Chawla, Ananthram Swami: metapath2vec: Scalable Representation Learning for Heterogeneous Networks. KDD 2017: 135-144
- Aleksandar Bojchevski, Stephan Günnemann: Deep Gaussian Embedding of Graphs: Unsupervised Inductive Learning via Ranking. ICLR 2018.

## Deep Graph Models

### Graph Autoencoders
- Kipf, Thomas N., and Max Welling. "Variational graph auto-encoders." arXiv preprint arXiv:1611.07308 (2016).
- Wang, D.; Cui, P.; Zhu, W. Structural Deep Network Embedding. In Proceedings of the 22nd International Conference on Knowledge Discovery and Data Mining (SIGKDD 2016); Association for Computing Machinery: New York, NY, USA, 2016; KDD ’16, p. 1225–1234. https://doi.org/10.1145/2939672.2939753. 
- Tu, K.; Cui, P.; Wang, X.; Wang, F.; Zhu, W. Structural Deep Embedding for Hyper-Networks. In Proceedings of the 32nd Conference on Artificial Intelligence (AAAI 2018); AAAI Press: New Orleans, Louisiana, USA, 2018; pp. 426–433.

### Spatial GNNs
- Thomas N. Kipf, Max Welling: Semi-Supervised Classification with Graph Convolutional Networks, ICLR 2017
- Hamilton, W.L.; Ying, Z.; Leskovec, J. Inductive Representation Learning on Large Graphs. In Proceedings of the 30th Annual Conference on Neural Information Processing Systems (NIPS 2017); 2017; pp. 1024–1034
- Chen, J.; Ma, T.; Xiao, C. FastGCN: Fast Learning with Graph Convolutional Networks via Importance Sampling. In Proceedings of the 6th International Conference on Learning Representations (ICLR 2018); OpenReview.net: Vancouver, BC, Canada, 2018 
- Chiang, W.; Liu, X.; Si, S.; Li, Y.; Bengio, S.; Hsieh, C. Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph Convolutional Networks. In Proceedings of the 25th International Conference on Knowledge Discovery & Data Mining (KDD 2019); ACM: Anchorage, Alaska, USA, 2019; pp. 257–266. https://doi.org/10.1145/3292500.3330925.
- Li, G.; Xiong, C.; Thabet, A.K.; Ghanem, B. DeeperGCN: All You Need to Train Deeper GCNs. CoRR 2020, abs/2006.07739 [2006.07739].
- Chen, M.; Wei, Z.; Huang, Z.; Ding, B.; Li, Y. Simple and Deep Graph Convolutional Networks. In Proceedings of the 37th International Conference on Machine Learning (ICML 2020); PMLR: Virtual Event, 2020; Vol. 119, Proceedings of Machine Learning Research, pp. 1725–1735
- Xu, Keyulu, Weihua Hu, Jure Leskovec, and Stefanie Jegelka. "How powerful are graph neural networks?." arXiv preprint arXiv:1810.00826 (2018).

### Attentive GNNs
- Petar Velickovic, Guillem Cucurull, Arantxa Casanova, Adriana Romero, Pietro Liò, Yoshua Bengio: Graph Attention Networks. CoRR abs/1710.10903 (2017)
- Hong, X., Li, W., Wang, C., Lin, M., & Lu, S. Label attentive distillation for GNN-based graph classification. AAAI  2024.
- Yang Ye, Shihao Ji: Sparse Graph Attention Networks. IEEE Trans. Knowl. Data Eng. 35(1): 905-916 (2023)
- Kim, D.; Oh, A. How to Find Your Friendly Neighborhood: Graph Attention Design with Self-Supervision. In Proceedings of the 9th International Conference on Learning Representations; ICLR 2021.
- Shaked Brody, Uri Alon, Eran Yahav: How Attentive are Graph Attention Networks? ICLR 2022

### Limitations of GNNs and Their Solutions

#### GNNs with Scalability
- Chen, J.; Ma, T.; Xiao, C. FastGCN: Fast Learning with Graph Convolutional Networks via Importance Sampling. In Proceedings of the 6th International Conference on Learning Representations (ICLR 2018); OpenReview.net: Vancouver, BC, Canada, 2018 
- Chiang, W.; Liu, X.; Si, S.; Li, Y.; Bengio, S.; Hsieh, C. Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph Convolutional Networks. In Proceedings of the 25th International Conference on Knowledge Discovery & Data Mining (KDD 2019); ACM: Anchorage, Alaska, USA, 2019; pp. 257–266. https://doi.org/10.1145/3292500.3330925.
- Li, G.; Xiong, C.; Thabet, A.K.; Ghanem, B. DeeperGCN: All You Need to Train Deeper GCNs. CoRR 2020, abs/2006.07739 [2006.07739].
- Chen, M.; Wei, Z.; Huang, Z.; Ding, B.; Li, Y. Simple and Deep Graph Convolutional Networks. In Proceedings of the 37th International Conference on Machine Learning (ICML 2020) 
- Kezhi Kong, Jiuhai Chen, John Kirchenbauer, Renkun Ni, C. Bayan Bruss, and Tom Goldstein. GOAT: A Global Transformer On Large-scale Graphs. In Proceedings of the 40th International Conference on Machine Learning (ICML), pages 17375–17390, 2023.
- Chuang Liu, Yibing Zhan, Xueqi Ma, Liang Ding, Dapeng Tao, Jia Wu, and Wenbin Hu. Gapformer: Graph Transformer With Graph Pooling For Node Classification. In Proceedings of the Thirty-Second International Joint Conference on Artificial Intelligence (IJCAI), pages 2196–2205, 2023.
- Chen, Jinsong, Kaiyuan Gao, Gaichao Li, and Kun He. "NAGphormer: A tokenized graph transformer for node classification in large graphs." ICRL 2023.

#### GNNs with Fairness
- Jiang, Zhimeng, et al. "Chasing Fairness in Graphs: A GNN Architecture Perspective." Proceedings of the AAAI Conference on Artificial Intelligence. Vol. 38. No. 19. 2024.
- Wang, Ruijia, et al. "Uncovering the structural fairness in graph contrastive learning." Advances in neural information processing systems 35 (2022): 32465-32473.
- Liu, Zemin, Trung-Kien Nguyen, and Yuan Fang. "On generalized degree fairness in graph neural networks." Proceedings of the AAAI Conference on Artificial Intelligence. Vol. 37. No. 4. 2023.
- Pan, Chenglu, et al. "Towards fair graph federated learning via incentive mechanisms." Proceedings of the AAAI Conference on Artificial Intelligence. Vol. 38. No. 13. 2024.
- Renqiang Luo, Huafei Huang, Shuo Yu, Xiuzhen Zhang, Feng Xia. Fairgt: A fairness-aware graph transformer. IJCAI 2024.
- Liu, Z., Qiu, R., Zeng, Z., Yoo, H., Zhou, D., Xu, Z., ... & Tong, H. Class-imbalanced graph learning without class rebalancing. ICRL 2024.

#### GNNs with Heterophily
- Wang, Junfu, et al. "Understanding heterophily for graph neural networks." ICRL 2024
- Park, MoonJeong, Jaeseung Heo, and Dongwoo Kim. "Mitigating oversmoothing through reverse process of gnns for heterophilic graphs." arXiv preprint arXiv:2403.10543 (2024).
- Wu, Yuhao, Jiangchao Yao, Bo Han, Lina Yao, and Tongliang Liu. "Unraveling the impact of heterophilic structures on graph positive-unlabeled learning." ICRL 2024
- Luan, Sitao, Chenqing Hua, Qincheng Lu, Jiaqi Zhu, Mingde Zhao, Shuyuan Zhang, Xiao-Wen Chang, and Doina Precup. "Revisiting heterophily for graph neural networks." Advances in neural information processing systems 35 (2022): 1362-1375.
- Zhu, Jiong, et al. "Graph neural networks with heterophily." Proceedings of the AAAI conference on artificial intelligence. Vol. 35. No. 12. 2021.

#### GNNs with Long-Range Dependency
- Bamberger, J., Gutteridge, B., Roux, S. L., Bronstein, M. M., & Dong, X. (2025). On Measuring Long-Range Interactions in Graph Neural Networks. arXiv preprint arXiv:2506.05971.
- Susheel Suresh, Vinith Budde, Jennifer Neville, Pan Li, Jianzhu Ma: Breaking the Limit of Graph Neural Networks by Improving the Assortativity of Graphs with Local Mixing Patterns. KDD 2021
- Wu, Zhanghao, et al. "Representing long-range context for graph neural networks with global attention." Advances in neural information processing systems 34 (2021): 13266-13279.
- Chen, Dexiong, Till Hendrik Schulz, and Karsten Borgwardt. "Learning long range dependencies on graphs via random walks." ICLR 2025
- Wu, Zhanghao, et al. "Representing long-range context for graph neural networks with global attention." Advances in neural information processing systems 34 (2021): 13266-13279.

#### Over-smoothing Problems
- Park, M., Choi, S., Heo, J., Park, E., & Kim, D. (2025). The Oversmoothing Fallacy: A Misguided Narrative in GNN Research. arXiv preprint arXiv:2506.04653.
- Juan Shu, Bowei Xi, Yu Li, Fan Wu, Charles A. Kamhoua, Jianzhu Ma: Understanding Dropout for Graph Neural Networks. WWW 2022
- Chen, Deli, et al. "Measuring and relieving the over-smoothing problem for graph neural networks from the topological view." Proceedings of the AAAI conference on artificial intelligence. Vol. 34. No. 04. 2020. 
- Keriven, Nicolas. "Not too little, not too much: a theoretical analysis of graph (over) smoothing." Advances in Neural Information Processing Systems 35 (2022): 2268-2281.
- Liu, Meng, Hongyang Gao, and Shuiwang Ji. "Towards deeper graph neural networks." Proceedings of the 26th ACM SIGKDD international conference on knowledge discovery & data mining. 2020.
- Zhou, Kaixiong, et al. "Towards deeper graph neural networks with differentiable group normalization." Advances in neural information processing systems 33 (2020): 4917-4928.

#### Over-squarshing Problems
- Giraldo, Jhony H., et al. "On the trade-off between over-smoothing and over-squashing in deep graph neural networks." Proceedings of the 32nd ACM international conference on information and knowledge management. 2023.
- Z. Ying, J. You, C. Morris, X. Ren, W. Hamilton, J. Leskovec, Hierarchical graph representation learning with differentiable pooling, Adv. Neural Inf. Process. Syst. 31 (2018)
- C. Sanders, A. Roth, T. Liebig, Curvature-based pooling within graph neural networks, 2023, arXiv preprint arXiv:2308.16516.
-  Liu, Yang, Chuan Zhou, Shirui Pan, Jia Wu, Zhao Li, Hongyang Chen, and Peng Zhang. "Curvdrop: A ricci curvature based approach to prevent graph neural networks from over-smoothing and over-squashing." In Proceedings of the ACM Web Conference 2023, pp. 221-230. 2023.
- Di Giovanni, Francesco, et al. "On over-squashing in message passing neural networks: The impact of width, depth, and topology." International conference on machine learning. PMLR, 2023. 
- Alon, Uri, and Eran Yahav. "On the bottleneck of graph neural networks and its practical implications." ICRL 2021.

#### Over-globalizing Problems in Graph Transformers
- Xing, Yujie, et al. "Less is more: on the over-globalizing problem in graph transformers." arXiv preprint arXiv:2405.01102 (2024).
- Yadati, Naganand. "Localformer: Mitigating over-globalising in transformers on graphs with localised training." Transactions on Machine Learning Research (2025).
- Wu, Q., Zhao, W., Yang, C., Zhang, H., Nie, F., Jiang, H., Bian, Y., and Yan, J. Simplifying and empowering transformers for large-graph representations. In Thirty seventh Conference on Neural Information Processing Systems, 2023.


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


