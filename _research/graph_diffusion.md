---
title: "Diffusion on graphs"
layout: single-portfolio
excerpt: "<img src='/images/research/multiscale.png' alt=''>"
collection: research
order_number: 50
---

Diffusion is a common method for examining the structure and modelling physical processes on graphs. No differently, I have been interested in diffusion on graphs to solve various problems. In particular, I have been interested in the transient responses of nodes to diffusion at some source. Using the transient responses of other nodes we can extract lots of interesting information about the graph and also perform node classification.

<p align="center">
  <img src="/images/research/diffusion.png" height="100px" width="600px" />
</p>

The below set of papers came from our investigations into the transient responses of nodes to diffusive sources.



## Multiscale Centrality

In the first project we constructed a measure of Multiscale Centrality:

> Classic measures of graph centrality capture distinct aspects of node importance, from the local(e.g., degree) to the global (e.g., closeness). Here we exploit the connection between diffusion andgeometry to introduce a multiscale centrality measure. A node is defined to be central if it breaks the metricity of the diffusion as a consequence of the effective boundaries and inhomogeneities in the graph. Our measure is naturally multiscale, as it is computed relative to graph neighbourhoods within the varying time horizon of the diffusion. We find that the centrality of nodes can differ widely at different scales. In particular, our measure correlates with degree (i.e., hubs) at smallscales and with closeness (i.e., bridges) at large scales, and also reveals the existence of multi-centric structures in complex networks. By examining centrality across scales, our measure thus provides an evaluation of node importance relative to local and global processes on the network.

<p align="center">
  <img src="/images/research/multiscale.png" height="400px" width="600px" />
</p>

[Article](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.2.033104){: .btn--research} 


## Graph diffusion reclassification (GDR)

We then turned our attention to the problem of node classification but whilst retaining the notion of diffusion. The software for GDR can be found [here](https://github.com/barahona-research-group/GDR).

Classification tasks based on feature vectors can be significantly improved by including within deep learning a graph that summarises pairwise relationships between the samples. Intuitively, the graph acts as a conduit to channel and bias the inference of class labels. Here, we study classification methods that consider the graph as the originator of an explicit graph diffusion. We show that appending graph diffusion to feature-based learning as an a posteriori refinement achieves state-of-the-art classification accuracy. This method, which we call Graph Diffusion Reclassification (GDR), uses overshooting events of a diffusive graph dynamics to reclassify individual nodes. The method uses intrinsic measures of node influence, which are distinct for each node, and allows the evaluation of the relationship and importance of features and graph for classification.

<p align="center">
  <img src="/images/research/gdr.png" height="400px" width="600px" />
</p>


[Article](https://www.aimsciences.org/article/doi/10.3934/fods.2020002){: .btn--research} 




