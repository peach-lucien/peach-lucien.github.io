---
title: "Diffusion on graphs"
layout: single-portfolio
excerpt: "<img src='/images/research/multiscale.png' alt=''>"
collection: research
order_number: 1
---

Diffusion is a common method for examining the structure and modelling physical processes on graphs. No differently, I have been interested in diffusion on graphs to solve various problems. In particular, I have been interested in the transient responses of nodes to diffusion at some source. Using the transient responses of other nodes we can extract lots of interesting information about the graph and also perform node classification.

<p align="center">
  <img src="/images/research/diffusion.png" height="100px" width="600px" />
</p>

The below set of papers came from our investigations into the transient responses of nodes to diffusive sources.

## Relative Dimension

Probably the most interesting output from our exploration into diffusion, geometry and graph structures was the definition of Relative Dimension. Dimension is a fundamental concept within physics and mathematics that characterizes objects and the spaces in which they are embedded, and has many important physical consequences. Yet in many real-world, complex physical systems, the ideal notion of dimension does not extend easily to many real-world, complex physical systems, in which the spaces under consideration can be finite with boundaries; may be bounded, inhomogeneous; or can be intrinsically discrete (as in networks), thus any processes within the space are constrained. Here we introduce a dynamics-based notion of dimension that applies naturally to such non-ideal physical systems.

<p align="center">
  <img src="/images/research/dimension_figure_schematic.png" height="400px" width="600px" />
</p>


Our work exploits the classic link between diffusive processes and the geometry of the space in which they evolve. Classically, Indeed, diffusion has been used to examine the geometry of such spaces, and through observation of the  the observation of diffusion behaviour one can be used to reveal the dimension of the space in which it occurs . For example, by considering, e.g., the speed of decay of the decay of a delta function at a point.  at a some source  then one can extract an estimate of the dimension (S. Reuveni, R. Granek, and J. Klafter, Proceedings of the National Academy of Sciences, 107, 13696, 2010).  However, existing such approaches  to measuring dimension, such as that cited, only consider the dynamics at one point - the source of the delta function. In contrast, our in this paper we introduce a notion of dimension that exploits the propagation of the diffusion, i.e., we compute the dimension from the observation of ing the transient response at a  some different point yi different fromto the source y0. Accordingly, the dimension is relative between the source and observer, and forms the basis of our conceptualisation of relative dimension. This Importantly, our approach enriches the notion of dimension, a statement which we illustrate through a simple constructed example in which we consider a 2-d filled circle attached to a 1-d line. We can initialise a delta function at the joint between the circle and line and then measure the dimension at y1 in the centre of the circle and y2 at the end of the 1-d line. The relative dimension of the source to y1 would be closer to ~2, whilst closer to ~1 when measuring relative to y2. Had we only considered the source, and not the propagation of diffusion, we would have ignored these crucial differences stemming from the relative geometry between each pair of points.

Being built from simple considerations on Euclidean spaces, we recover the expected Euclidean dimension for infinite regular grids while providing a unique tool to study graphs from an intrinsic and fundamental physical principle. In addition, we have constructed two other measures, the local and global dimensions, by averaging the relative dimension with a notion of scale. In our [paper](https://arxiv.org/abs/2106.05368), we showcase all three measures with various examples, from simple grids to allostery in proteins or epidemic spreading, where, in each, they have their own physical interpretation and practical use for analysis or predictions problems. We provide a [Python package](https://github.com/barahona-research-group/DynGDim) for easy implementation of our method.

 



## Multiscale Centrality

In the first project we constructed a measure of Multiscale Centrality. In this project, we wanted to capture the essence of scale within a centrality measure. There existed other centrality measures that touched on this idea, but never formalised the notion of scale. Here, we show that scale is fundamental when examining node centrality and introduce a methodology for scanning through the scales of a network.

> Classic measures of graph centrality capture distinct aspects of node importance, from the local(e.g., degree) to the global (e.g., closeness). Here we exploit the connection between diffusion andgeometry to introduce a multiscale centrality measure. A node is defined to be central if it breaks the metricity of the diffusion as a consequence of the effective boundaries and inhomogeneities in the graph. Our measure is naturally multiscale, as it is computed relative to graph neighbourhoods within the varying time horizon of the diffusion. We find that the centrality of nodes can differ widely at different scales. In particular, our measure correlates with degree (i.e., hubs) at smallscales and with closeness (i.e., bridges) at large scales, and also reveals the existence of multi-centric structures in complex networks. By examining centrality across scales, our measure thus provides an evaluation of node importance relative to local and global processes on the network.

<p align="center">
  <img src="/images/research/multiscale.png" height="400px" width="600px" />
</p>

[Article](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.2.033104){: .btn--research} 


## Graph diffusion reclassification (GDR)

We then turned our attention to the problem of node classification but whilst retaining the notion of diffusion. The software for GDR can be found [here](https://github.com/barahona-research-group/GDR). Prior to this project, node classification problems used the idea of message passing to learning network structures - here we wanted to use explicit diffusion dynamics to uncover the subtleties of network structure to improve node classification.

Classification tasks based on feature vectors can be significantly improved by including within deep learning a graph that summarises pairwise relationships between the samples. Intuitively, the graph acts as a conduit to channel and bias the inference of class labels. Here, we study classification methods that consider the graph as the originator of an explicit graph diffusion. We show that appending graph diffusion to feature-based learning as an a posteriori refinement achieves state-of-the-art classification accuracy. This method, which we call Graph Diffusion Reclassification (GDR), uses overshooting events of a diffusive graph dynamics to reclassify individual nodes. The method uses intrinsic measures of node influence, which are distinct for each node, and allows the evaluation of the relationship and importance of features and graph for classification.

<p align="center">
  <img src="/images/research/gdr.png" height="400px" width="600px" />
</p>


[Article](https://www.aimsciences.org/article/doi/10.3934/fods.2020002){: .btn--research} 




