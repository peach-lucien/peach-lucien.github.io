---
title: "Machine learning and graphs"
layout: single-portfolio
excerpt: "<img src='/images/research/hcga_workflow.png' alt=''>"
collection: research
order_number: 50
---

The interface between machine-learning and graphs is growing quickly. 

> Machine learning on graphs is an important and ubiquitous task with applications ranging from drug design to friendship recommendation in social networks. The primary challenge in this domain is finding a way to represent, or encode, graph structure so that it can be easily exploited by machine learning models. Traditionally, machine learning approaches relied on user-defined heuristics to extract features encoding structural information about a graph (e.g., degree statistics or kernel functions). However, recent years have seen a surge in approaches that automatically learn to encode graph structure into low-dimensional embeddings, using techniques based on deep learning and nonlinear dimensionality reduction. 

To support this effort a number of my research projects have explored how diffusion can be used on graphs to improve node classification or standard graph theoretical metrics can be used for graph classification.



## Graph diffusion reclassification (GDR)

We first explored node classification. The software for GDR can be found [here](https://github.com/barahona-research-group/GDR).

> Classification tasks based on feature vectors can be significantly improved by including within deep learning a graph that summarises pairwise relationships between the samples. Intuitively, the graph acts as a conduit to channel and bias the inference of class labels. Here, we study classification methods that consider the graph as the originator of an explicit graph diffusion. We show that appending graph diffusion to feature-based learning as an a posteriori refinement achieves state-of-the-art classification accuracy. This method, which we call Graph Diffusion Reclassification (GDR), uses overshooting events of a diffusive graph dynamics to reclassify individual nodes. The method uses intrinsic measures of node influence, which are distinct for each node, and allows the evaluation of the relationship and importance of features and graph for classification.


[Article](https://www.aimsciences.org/article/doi/10.3934/fods.2020002){: .btn--research} 

## Highly Comparative Graph Analysis (HCGA)

We then moved our attention to graph classification. We noticed that deep-learning methods were quite poor and there was no existing benchmark for comparison. Therefore we developed hcga - a [software package](https://github.com/barahona-research-group/hcga) for graph feature extraction:

> Networks are widely used as mathematical models of complex systems across many scientific disciplines, not only in biology and medicine but also in the social sciences, physics, computing and engineering. Decades of work have produced a vast corpus of research characterising the topological, combinatorial, statistical and spectral properties of graphs. Each graph property can be thought of as a feature that captures important (and some times overlapping) characteristics of a network. In the analysis of real-world graphs, it is crucial to integrate systematically a large number of diverse graph features in order to characterise and classify networks, as well as to aid network-based scientific discovery. Here, we introduce hcga, a framework for highly comparative analysis of graph data sets that computes several thousands of graph features from any given network. hcga also offers a suite of statistical learning and data analysis tools for automated identification and selection of important and interpretable features underpinning the characterisation of graph data sets.

<p align="center">
  <img src="/images/research/hcga_workflow.png" height="400px" width="800px" />
</p>


[Article](https://doi.org/10.1016/j.patter.2021.100227){: .btn--research} 







