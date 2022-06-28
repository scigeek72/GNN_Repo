# GNN_Repo
Contains reference papers and other info related to Graph Neural Network

# Papers (in random order)
- [Identity Aware Graph Neural Nets](https://arxiv.org/pdf/2101.10320.pdf) by You, Gomes-Selman, Ying, Leskovec (2021)
- [Design Space for Graph Neural Networks](https://arxiv.org/pdf/2011.08843.pdf) by You, Ying, Leskovec (2021)
- [Learning Structural Node Embeddings via Diffusion Wavelets](https://arxiv.org/pdf/1710.10321.pdf) by Donnat, Zitnik, Hallac, Leskovec(2018) 
  - Node embeddings that also incorporate *structural* properties of the nodes (such as hubs). Very Interesting but *may* require more work.
- [Exploiting Edge features in Graph Neural Networks](https://arxiv.org/pdf/1809.02709.pdf)
- [Neural Message Passing in Quantum Chemistry](https://arxiv.org/pdf/1704.01212.pdf) by Gilmer et.al
  - Consider Message Passing using *edge-features*
- [Relational inductive biases, deep learning, and graph networks](https://arxiv.org/abs/1806.01261) by . Battaglia et.al
  - Consider Message passing using *edge-features*
- [NENN: Incorporate Edge and Node Features in Graph Neural Networks](http://proceedings.mlr.press/v129/yang20a/yang20a.pdf) by Yang, Li (2020)
- [Principal Neighborhood Aggregation for graph nets](https://docs.google.com/viewer?url=https%3A%2F%2Farxiv.org%2Fpdf%2F2004.05718.pdf)
- **Survey** [A comprehensive Survey on Graph Neural Networks](https://arxiv.org/pdf/1901.00596.pdf)
- [DeepWalk: Online Learning of Social Representation](https://arxiv.org/pdf/1403.6652.pdf)
- [Node2vec: Scalable Feature Learning For Networks](https://arxiv.org/abs/1607.00653)
- [GraphSAGE: Inductive Representation Learning on Large Graphs](https://arxiv.org/abs/1706.02216) by Hamilton, Ying, Leskovec 
  - Reviews are good. **Inductive and not transductive** can work on previously unseen nodes.
  - No edge-features were considered for Node embedding (so, look at the following paper in this list)
- [E-GraphSAGE: A Graph Neural Networks based Intrusion Detection System for IoT](https://arxiv.org/abs/2103.16329) 
  - On computer networks
- **Survey** [Graph Neural Networks: A review of methods and application](https://arxiv.org/abs/1812.08434)  
- [Graph Attention Networks](https://arxiv.org/abs/1710.10903v3) 
- [NF-GNN:Network Flow Graph for Malware Detection and classification](https://arxiv.org/pdf/2103.03939.pdf)
  - On computer networks
  - Incorporates *Edge-features* in the model
- [Residual Gated Graph ConvNets](https://arxiv.org/abs/1711.07553)
- [Crystal Graph Convolutional Neural Networks for an Accurate and
Interpretable Prediction of Material Properties](https://arxiv.org/pdf/1710.10324.pdf)
  - Incorporates *EDGE-features* in the model
- [Edge Attention based Multi-relational Graph Convolutional Networks](https://arxiv.org/pdf/1802.04944v1.pdf) 
  - An extension of the Graph Attention Network (see blog: Graph attention network for more comments)
- [How powerful are Graph Neural Networks?](https://arxiv.org/abs/1810.00826) by Leskovec, Jagelka
  - assess different aggregation functions (excellent review on [Openreview.net](https://openreview.net/forum?id=ryGs6iA5Km))

# Books and Book Chapters
- [Graph Reprenstation Learning](https://www.cs.mcgill.ca/~wlh/grl_book/) by William Hamilton 
- [Graph Neural Networks: Foundation, Frontiers and Applications](https://graph-neural-networks.github.io/#tab-part3)
  - All the chapters are available (including on Anomaly detection which I am listing below seperately) written some of the leading researchers  in the field
- **Book Chapter** [Graph Neural Networks in Anomaly Detection](https://graph-neural-networks.github.io/static/file/chapter26.pdf) by Shen Wang, Philip S. Yu

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

# Related Videos
- **Youtube: [How to use edge-features in GNN](https://www.youtube.com/watch?v=mdWQYYapvR8)**
  - Nice visualization and summary of the important message passing concepts that incorporate *multi-dimensional Edge features* from various papers (including pytorch modules and how to incorporate edge-features/edge-attributes into GNN code)
-  **Youtube: [Geometric Deep Learning on Graphs](https://www.youtube.com/watch?v=b187J4ndZWY&list=WL&index=92&t=20s)** by Michael Bronstein
-  **Youtube: [Intro to GNN](https://www.youtube.com/watch?v=8owQBFAHw7E)** by Petar Veličković 
-  **Youtube: [Intro to GNN: Model and Applications](https://www.youtube.com/watch?v=zCEYiCxrL_0)** by Microsoft Research (Not very informative)  

# Python Libraries to work with Graphs
- [DGL Documentation](https://docs.dgl.ai/index.html) and [DGL code base](https://github.com/dmlc/dgl)
  - Can be used with Pytorch, Tensorflow and MaxNet. Try this First
- [GraphNets](https://github.com/deepmind/graph_nets) 
  - From DeepMind. Tensorflow based high quality modules (try to use this instead of Stellar Graphs). 
- [Stellar Graphs](https://stellargraph.readthedocs.io/en/stable/README.html)
  - Tensorflow + Keras based. 
- [Pytorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/modules/nn.html)
  - Pytorch based  


# Other Resources
- [DeepSnap](https://snap.stanford.edu/deepsnap/)
- [GraphGym](https://github.com/snap-stanford/GraphGym) and [PyG](https://www.pyg.org/)
  - Based on Pytorche. **PyG** is a more tightly integrated version of **GraphGym** 
- [SNAP: Stanford Network Analysis Project](http://snap.stanford.edu/index.html)
