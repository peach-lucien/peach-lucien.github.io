---
layout: archive
title: Code
permalink: /Code/
---
<script>addBackToTop({
  backgroundColor: '#fff',
  innerHTML: 'Back to Top',
  textColor: '#333'
})</script>
<style>
  #back-to-top {
    border: 1px solid #ccc;
    border-radius: 0;
    font-family: sans-serif;
    font-size: 14px;
    width: 100px;
    text-align: center;
    line-height: 30px;
    height: 30px;
  }
</style>
Below you find brief descriptions and the links to code related to several projects.

* [Data-driven clustering of time-series](#DDCBEHAVIOURS)
* [Highly Comparative Graph Analysis](#HCGA)
* [MarkovTrap: semi-supervised learning on graphs](#MARKOVTRAP)
* [ Predicting the effect of protein mutations using graph theory](#ADK1)


## Data-driven clustering of student engagement time-series to identify learning behaviours
{: #DDCBEHAVIOURS}
Here, we present an unsupervised methodology that allows the direct analysis of raw time series gathered from the engagement of learners as they complete tasks of online courses without imposing a priori the number or type of groups of learners, i.e., distinct learner clusters are not pre-determined nor identified subjectively based on prior features but are detected algorithmically during the data analysis. Specifically, we analysed the time series (i.e., time stamped data of task completion) of 81 learners as they undertook the six online compulsory courses that form the first year of a2-year part-time postgraduate management degree.  The courses extended over three terms and the patterns of task completion differ greatly across the learner group.

The methodology we implemented is summarised in the below Figure. Using the time stamps of task completion by each learner, we employ adynamic time warping kernel to calculate similarities between learner time series and construct a similarity score between all pairs of learners. From this information, we then construct a similarity graph of the learner group and apply to it Markov Stability, a multiscale unsupervised graph partitioning framework, in order to obtain clusters of learners with similar temporal behaviours.

<div style="border: 1px solid black; padding: 0px;" markdown="1">
![image-center](/images/DTW_clustering.png){: .align-center}
</div>


\[1] Peach, Robert L. and Yaliraki, Sophia N. and Lefevre, David and Barahona, Mauricio.
" Data-driven unsupervised clustering of online learner behaviour " 
*arXiv preprint*, 2019, [DOI: arXiv:1902.04047](https://arxiv.org/abs/1902.04047)   






## Highly Comparative Graph Analysis (hcga)
{: #HCGA}
Classification of graphs is both of interest but difficult to achieve. In recent years, a variety of deep learning methodologies have been developed that attempt to learn graph features. These methods either try and learn the spectral decomposition of a network or apply convolutional architectures. However, these methods inherently bias themselves the static representation of the graph and don't learn long distance features. For example, convolutional architectures learn local features based on nearest or next nearest neighbours. Moreover, these deep learning methodologies provide little information about the graph features which are most important for classification which prevents informed graph design.

To overcome this failing we have developed hcga: Highly comparative graph analysis. Taking inspiration from hctsa (Highly comparative time-series analysis) we have developed a Python package that undiscriminantly calculates 1000s of graph features. This enables simple machine learning methods to predict the class of graphs. Moreover, the massive feature extraction enables the user to identify specific features which enable high classification accuracy and can provide insight into the differences between graph classes.

[https://imperialcollegelondon.github.io/hcga/](https://imperialcollegelondon.github.io/hcga/)  



## MarkovTrap: Semi-supervised learning on graphs
{: #MARKOVTRAP}

Networks can provide a concise, elegant and powerful representation of complex systems. In recent years, there has been a surge of interest in network analysis that has provided a wide range of analytical tools. Typically, these methods aim to reveal the structural properties of the network that can be used to infer the behaviour of the system which the network describes. Most literature in network science focuses solely on the topology of the network; tools are developed to reveal information about the nodes and the edges that link them. However, in most applications, the network will be accompanied by additional information that describes the nodes (or edges). The atom type or charge in a molecule network, the website text on an internet network, the demographic background of a person on a social network, are all examples of important information that are often disregarded in standard network analyses. 

Despite there often being a wealth of meta-data for each node, often the majority of a network will be unlabelled. For example, the minority of proteins in a protein-protein interaction network may be of known function, or the minority of persons within a social network may be of known political inclination. Instead, the remaining labels must be inferred or learned from the network topology and metadata - this is commonly known as semi-supervised learning. It is important to emphasise the difference between meta-data and labels, where the former describes additional information about nodes and the latter describes a `ground truth' representation of the network. The meta-data is not necessarily an appropriate proxy for the node labels. 

We introduce MarkovTrap, an intuitive dynamical approach for semi-supervised learning on graphs based on Markovian random-walks. Instead of learning the class labels using a non-linear graph convolutional method, MarkovTrap uses a dynamic Markov process of the class labels across the graph. 
The feature information is incorporated into a prior probability distribution of the class labels through a cosine similarity function or an standard learned estimation. The diffusion is intrinsically related to the time scale of the random-walks and thus the class labels become transiently trapped in the underlying network structure, thus creating significant label propagation on non-neighbouring nodes. We apply this methodology to some of the standard citation networks and a wikipedia datasets to demonstrate that MarkovTrap gives similar accuracies to the state of the art graph convolutional neural networks. We also show that MarkovTrap is capable of classifying nodes on a directed network. 

<div style="border: 1px solid black; padding: 0px;" markdown="1">
![image-center](/images/toy_model_markovtrap.png){: .align-center}
</div>



## Predicting the effect of protein mutations using graph theory
{: #ADK1}

Proteins exhibit complex dynamics across a vast range of time and length scales, from the atomistic to the conformational. Adenylate kinase (ADK) showcases the biological relevance of such inherently coupled dynamics across scales: single mutations can affect large-scale protein motions and enzymatic activity. Here we present a combined computational and experimental study of multiscale structure and dynamics in proteins, using ADK as our system of choice. We show how a computationally efficient method for unsupervised graph partitioning can be applied to atomistic graphs derived from protein structures to reveal intrinsic, biochemically relevant substructures at all scales, without re-parameterisation or a priori coarse-graining. We subsequently perform full alanine and arginine in silico mutagenesis scans of the protein, and score all mutations according to the disruption they induce on the large-scale organisation. We use our calculations to guide FRET experiments on ADK, and show that mutating residue D152 to alanine or residue V164 to arginine induce a large dynamical shift of the protein structure towards a closed state, in accordance with our predictions. Our computations also predict a graded effect of different mutations at the D152 site as a result of increased coherence between the core and binding domains, an effect confirmed quantitatively through a high correlation ( R2 = 0.93 ) with the FRET ratio between closed and open populations measured on six mutants.

<div style="border: 1px solid black; padding: 0px;" markdown="1">
![image-center](/images/ADK_results.png){: .align-center}
</div>

