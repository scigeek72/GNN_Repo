# GNN_Repo
Contains reference papers and other info related to Graph Neural Network

# Papers (in random order)
- [Benchmarking Node Outlier Detection on Graphs](https://arxiv.org/pdf/2206.10071.pdf) by Liu et.al
- [Graph Representation Learing in Biomedicine](https://arxiv.org/pdf/2104.04883.pdf) by Li, Huang, Zitnik
- [Modeling Relational Data with Graph Convolutional Network](https://arxiv.org/pdf/1703.06103.pdf) By Schlichtkrull, Kipf, Welling, Bloom, Titov, van der Berg
- [Fast Graph Representation Learning with PyTorch-Geometric](https://docs.google.com/viewer?url=https%3A%2F%2Frlgm.github.io%2Fpapers%2F2.pdf) by Mathew Fay et.al
- [Graph Convolutional Networks for Graph with Multi-dimensionally weighted edges](https://cims.nyu.edu/~chenzh/files/GCN_with_edge_weights.pdf) by Chen (July 20, 2020)
- [Strategies for Pre-Training Graph Neural Networks](https://arxiv.org/pdf/1905.12265.pdf) by Hu, Liu, Gomes, Zitnik, Liang, Pande, and Leskovec
  - Interesting paper on pretraining strategies for performance enhancement
  - Has implementation in PyG (look [here](https://pytorch-geometric.readthedocs.io/en/latest/modules/nn.html#torch_geometric.nn.conv.GINEConv))  
- [ETA prediction using Graph Neural Networks in Google Maps](https://dl.acm.org/doi/epdf/10.1145/3459637.3481916) 
  - Very dense paper with a lot of innovations, includes *edge-features*. 
- [Graph Convolutional Neural Nets for Web-Scale Recommender System (PinSage)](https://arxiv.org/pdf/1806.01973.pdf) by Ying, He, Chen, Eksombatchai, Hamilton, Leskovec (2018)
  - PinSage is implemented and productionized at Pinterest. Graph Size is 3 billion Nodes and 18 billion Edges 
  - This paper has number of improvements on traditional GCN and GraphSage
- [Identity Aware Graph Neural Nets (ID-GNN)](https://arxiv.org/pdf/2101.10320.pdf) by You, Gomes-Selman, Ying, Leskovec (2021)
  - More general framework than GNN (see **Lecture 16** in CS224W course) and perform better for node/edge/graph level tasks. 
  - Can be implemented with PyG/DGL etc. But more complicated. So, first start out with the original GNN.
- [Design Space for Graph Neural Networks](https://arxiv.org/pdf/2011.08843.pdf) by You, Ying, Leskovec (2021)
- [Learning Structural Node Embeddings via Diffusion Wavelets](https://arxiv.org/pdf/1710.10321.pdf) by Donnat, Zitnik, Hallac, Leskovec(2018) 
  - Node embeddings that also incorporate *structural* properties of the nodes (such as hubs). Very Interesting but *may* require more work.
- [Exploiting Edge features in Graph Neural Networks](https://arxiv.org/pdf/1809.02709.pdf)
- [Neural Message Passing in Quantum Chemistry](https://arxiv.org/pdf/1704.01212.pdf) by Gilmer et.al
  - Consider Message Passing using *edge-features*
- [Relational inductive biases, deep learning, and graph networks](https://arxiv.org/abs/1806.01261) by . Battaglia et.al
  - Consider Message passing using *edge-features*
- [NENN: Incorporate Edge and Node Features in Graph Neural Networks](http://proceedings.mlr.press/v129/yang20a/yang20a.pdf) by Yang, Li (2020)
  - This is attention based algorithm. But they seems to be doing the right updates as opposed to E-GraphSAGE. Can we incorporate this idea in the way GraphSAGE does it but instead now we incorporates (and updates) edge-features as well?????
- [Principal Neighborhood Aggregation for graph nets](https://docs.google.com/viewer?url=https%3A%2F%2Farxiv.org%2Fpdf%2F2004.05718.pdf)

- [DeepWalk: Online Learning of Social Representation](https://arxiv.org/pdf/1403.6652.pdf)
- [Node2vec: Scalable Feature Learning For Networks](https://arxiv.org/abs/1607.00653)
- [GraphSAGE: Inductive Representation Learning on Large Graphs](https://arxiv.org/abs/1706.02216) by Hamilton, Ying, Leskovec 
  - Reviews are good. **Inductive and not transductive** can work on previously unseen nodes.
  - No edge-features were considered for Node embedding (so, look at the following paper in this list). 
  - **Use this algorithm. It can be trained in uspervised mode.**
- [E-GraphSAGE: A Graph Neural Networks based Intrusion Detection System for IoT](https://arxiv.org/abs/2103.16329) 
  - On computer networks
  - There **seems** to be a fundamental problem in the updates of nodes features using edge features (line 5 in the algorithm). It talks about edge-features from the previous layer (k-1), but never updates edge-features.
  - DON'T USE IT AS IS. MODIFY IT. 
  
- [Graph Attention Networks](https://arxiv.org/abs/1710.10903v3) 
- [Semi-Supervised Classification with Graph Convolutional Networks](https://arxiv.org/abs/1609.02907) by Kipf, Welling (2017)
- [Convolutional Neural Networks on Graphs with Fast Localized Spectral Filtering](https://arxiv.org/abs/1606.09375) by Defferrard, Bresson, Vandergheynst (2017)
- [NF-GNN:Network Flow Graph for Malware Detection and classification](https://arxiv.org/pdf/2103.03939.pdf)
  - On computer networks
  - Incorporates *Edge-features* in the model
- [Residual Gated Graph ConvNets](https://arxiv.org/abs/1711.07553)
- [Crystal Graph Convolutional Neural Networks for an Accurate and
Interpretable Prediction of Material Properties](https://arxiv.org/pdf/1710.10324.pdf)
  - Incorporates *EDGE-features* in the model
  - [Github repo (with Pytorch)](https://github.com/txie-93/cgcnn/tree/f42ab233c4ee0c416879d6bc2d22a264418413ad)
- [Edge Attention based Multi-relational Graph Convolutional Networks](https://arxiv.org/pdf/1802.04944v1.pdf) 
  - An extension of the Graph Attention Network (see blog: Graph attention network for more comments)
- [How powerful are Graph Neural Networks?](https://arxiv.org/abs/1810.00826) by Leskovec, Jagelka
  - assess different aggregation functions (excellent review on [Openreview.net](https://openreview.net/forum?id=ryGs6iA5Km))
- [UBER-GNN: A User-Based Embeddings Recommendation based on Graph Neural Networks (Uber Eats Recommender System)](https://arxiv.org/abs/2008.02546) by Huang, Bi, Wu, Wang, Xiao (2020)
- [Variational Graph Auto-encoders](https://arxiv.org/pdf/1611.07308.pdf) by Kipf, Welling

## Survey Papers
- [A comprehensive Survey on Graph Neural Networks](https://arxiv.org/pdf/1901.00596.pdf)
- [Graph Neural Networks: A review of methods and application](https://arxiv.org/abs/1812.08434)

# Books and Book Chapters
- [Graph Reprenstation Learning](https://www.cs.mcgill.ca/~wlh/grl_book/) by William Hamilton 
- [Graph Neural Networks: Foundation, Frontiers and Applications](https://graph-neural-networks.github.io/#tab-part3)
  - All the chapters are available (including on Anomaly detection which I am listing below seperately) written some of the leading researchers  in the field
- **Book Chapter** [Graph Neural Networks in Anomaly Detection](https://graph-neural-networks.github.io/static/file/chapter26.pdf) by Shen Wang, Philip S. Yu
- [Geometric Deep Learning](https://arxiv.org/pdf/2104.13478.pdf) by Bronstein, Bruna, Cohen, and Veličković4
  - Note: Very theoratical and mathy.   

# Courses, Tutorials and Blog posts
- [CS224W:Machine Learning with Graphs](https://web.stanford.edu/class/cs224w/)
- [Pytorch Geometric Module](https://pytorch-geometric.readthedocs.io/en/latest/notes/introduction.html)
  - Contains a good assemblage of links to tutorials and blogs. Particularly look at these two [Colab Notebooks and Video Tutorials](https://pytorch-geometric.readthedocs.io/en/latest/notes/colabs.html) and [External Resources](https://pytorch-geometric.readthedocs.io/en/latest/notes/resources.html) 
- **Blog: [A gentle introduction to Graph Neural Networks](https://distill.pub/2021/gnn-intro/#other-types-of-graphs-multigraphs-hypergraphs-hypernodes)**
  - Nice introductory explanation with pointers to actual papers
- **Blog: [Understanding Convolution on Graphs](https://distill.pub/2021/understanding-gnns/)** by Ameya Daigavane, Balaraman Ravindran, Gaurav Aggarwal
  - Nice explanation (how Polynomial filters (Graph Laplacian) are translated into *Message passing* concepts*. Also have important pointers to papers
- **Blog: [Understanding Graph Neural Networks](https://irhum.pubpub.org/pub/gnn/release/4)** by Irhum Safkat
  - Nice introductory explanation
- **Blog: [Graph Attention Networks](https://petar-v.com/GAT/)** by Petar Veličković
- **Blog: [Graph Convolutional Networks](https://tkipf.github.io/graph-convolutional-networks/)** by Thomas Kipf
- **Blog: [Food Discovery with Uber Eats: Using Graph Learning to Power Recommendations](https://eng.uber.com/uber-eats-graph-learning/)** by Jain, Liu, Sarda, Molino (2019)
  - For the actual paper, see the paper section above

# Related Videos
- **Youtube: [How to use edge-features in GNN](https://www.youtube.com/watch?v=mdWQYYapvR8)**
  - Nice visualization and summary of the important message passing concepts that incorporate *multi-dimensional Edge features* from various papers (including pytorch modules and how to incorporate edge-features/edge-attributes into GNN code)
-  **Youtube: [Geometric Deep Learning on Graphs](https://www.youtube.com/watch?v=b187J4ndZWY&list=WL&index=92&t=20s)** by Michael Bronstein
-  **Youtube: [Intro to GNN](https://www.youtube.com/watch?v=8owQBFAHw7E)** by Petar Veličković 
-  **Youtube: [Intro to GNN: Model and Applications](https://www.youtube.com/watch?v=zCEYiCxrL_0)** by Microsoft Research (Not very informative)  

# Python Libraries to work with Graphs
- [PyGOD](https://github.com/pygod-team/pygod) 
  - PyGOD is based on Pytorch and pytorch_geometric and used for `graph outlier detection`(`anomaly detection`)
- [DGL Documentation](https://docs.dgl.ai/index.html) and [DGL code base](https://github.com/dmlc/dgl)
  - Can be used with Pytorch, Tensorflow and MaxNet. Try this First
- [GraphNets](https://github.com/deepmind/graph_nets) 
  - From DeepMind. Tensorflow based high quality modules (try to use this instead of Stellar Graphs). 
- [Stellar Graphs](https://stellargraph.readthedocs.io/en/stable/README.html)
  - Tensorflow + Keras based. 
- [Pytorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/modules/nn.html)
  - Pytorch based  
## How to form a graph in Python?
- **Blog** [Working With Large Internal Link Graphs in Python](https://www.briggsby.com/large-internal-link-graphs-in-python) by Justin
- [Networkx Documentation](https://networkx.org/documentation/networkx-1.10/reference/readwrite.edgelist.html)


# Other Resources
- [DeepSnap](https://snap.stanford.edu/deepsnap/)
- [GraphGym](https://github.com/snap-stanford/GraphGym) and [PyG](https://www.pyg.org/)
  - Based on Pytorche. **PyG** is a more tightly integrated version of **GraphGym** 
- [SNAP: Stanford Network Analysis Project](http://snap.stanford.edu/index.html)

# CyberSecurity Datasets
- [CyberSecurity Datasets](http://ahlashkari.com/Datasets.asp) 
  - Look at CICandMal-2017 dataset (and other similar datasets)
- [Graph Datasets](https://paperswithcode.com/datasets?mod=graphs&task=graph-embedding&page=1)
