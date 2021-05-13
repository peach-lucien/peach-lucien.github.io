---
title: "Machine learning and graphs"
layout: single-portfolio
excerpt: "<img src='/images/research/hcga_workflow.png' alt=''>"
collection: research
order_number: 50
---

Diffusion is a common method for examining the structure and modelling physical processes on graphs. No differently, I have been interested in diffusion on graphs to solve various problems. In particular, I have been interested in the transient responses of nodes to diffusion at some source. Using the transient responses of other nodes we can extract lots of interesting information about the graph and also perform node classification. The below set of papers came from our investigations into the transient responses of nodes to diffusive sources.



## Graph diffusion reclassification (GDR)

We first explored node classification. The software for GDR can be found [here](https://github.com/barahona-research-group/GDR).

> Classification tasks based on feature vectors can be significantly improved by including within deep learning a graph that summarises pairwise relationships between the samples. Intuitively, the graph acts as a conduit to channel and bias the inference of class labels. Here, we study classification methods that consider the graph as the originator of an explicit graph diffusion. We show that appending graph diffusion to feature-based learning as an a posteriori refinement achieves state-of-the-art classification accuracy. This method, which we call Graph Diffusion Reclassification (GDR), uses overshooting events of a diffusive graph dynamics to reclassify individual nodes. The method uses intrinsic measures of node influence, which are distinct for each node, and allows the evaluation of the relationship and importance of features and graph for classification.


[Article](https://www.aimsciences.org/article/doi/10.3934/fods.2020002){: .btn--research} 

## Highly Comparative Graph Analysis (HCGA)

We then moved our attention to graph classification. We noticed that deep-learning methods were quite poor and there was no existing benchmark for comparison. Therefore we developed hcga - a [software package](https://github.com/barahona-research-group/hcga) for graph feature extraction:

> Networks are widely used as mathematical models of complex systems across many scientific disciplines, not only in biology and medicine but also in the social sciences, physics, computing and engineering. Decades of work have produced a vast corpus of research characterising the topological, combinatorial, statistical and spectral properties of graphs. Each graph property can be thought of as a feature that captures important (and some times overlapping) characteristics of a network. In the analysis of real-world graphs, it is crucial to integrate systematically a large number of diverse graph features in order to characterise and classify networks, as well as to aid network-based scientific discovery. Here, we introduce hcga, a framework for highly comparative analysis of graph data sets that computes several thousands of graph features from any given network. hcga also offers a suite of statistical learning and data analysis tools for automated identification and selection of important and interpretable features underpinning the characterisation of graph data sets.

[Article](https://doi.org/10.1016/j.patter.2021.100227){: .btn--research} 







