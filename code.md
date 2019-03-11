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

