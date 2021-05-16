---
title: "Learning Analytics"
layout: single-portfolio
excerpt: "<img src='/images/research/datadriven_student_clustering.png' alt=''>"
collection: research
order_number: 50
---

The widespread adoption of online courses opens opportunities for analysing learner behaviour and optimising web-based learning adapted to observed usage. In collaboration with the [EdTech group in Imperial Business School](https://www.imperial.ac.uk/business-school/about-us/edtech-lab/), I began working on data extracted from the learning management system. Our aim was to first understand how students transitioned through courses, and then to find ways to predict performance and later optimise the student experience.


## Data-driven clustering of students

In our first investigation we introduced a mathematical framework for the analysis of time-series of online learner engagement, which allows the identification of clusters of learners with similar online temporal behaviour directly from the raw data without prescribing a priori subjective reference behaviours. The method uses a dynamic time warping kernel to create a pair-wise similarity between time-series of learner actions, and combines it with an unsupervised multiscale graph clustering algorithm to identify groups of learners with similar temporal behaviour. To showcase our approach, we analyse task completion data from a cohort of learners taking an online post-graduate degree at Imperial Business School. Our analysis reveals clusters of learners with statistically distinct patterns of engagement, from distributed to massed learning, with different levels of regularity, adherence to pre-planned course structure and task completion. The approach also reveals outlier learners with highly sporadic behaviour. A posteriori comparison against student performance shows that, whereas high-performing learners are spread across clusters with diverse temporal engagement, low performers are located significantly in the massed learning cluster, and our unsupervised clustering identifies low performers more accurately than common machine learning classification methods trained on temporal statistics of the data. Finally, we test the applicability of the method by analysing two additional data sets: a different cohort of the same course, and time-series of different format from another university.



<p align="center">
  <img src="/images/research/datadriven_student_clustering2.png" height="800px" width="400px" />
</p>


[Article](https://doi.org/10.1038/s41539-019-0054-0){: .btn--research} 


## Graph diffusion reclassification (GDR)

To extend our clustering of students, we aimed to further characterise learner behaviours with Bayesian modelling. In this study we leverage the sequence data framework and show how data-driven analysis of temporal sequences of task completion in online courses can be used to characterise personal and group learners’ behaviors, and to identify critical tasks and course sessions in a given course design. We also introduce a recently developed probabilistic Bayesian model to learn sequential behaviours of students and predict student performance. The application of our data-driven sequence-based analyses to data from learners undertaking an on-line Business Management course reveals distinct behaviors within the cohort of learners, identifying learners or groups of learners that deviate from the nominal order expected in the course. Using course grades a posteriori, we explore differences in behavior between high and low performing learners.

 We find that high performing learners follow the progression between weekly sessions more regularly than low performing learners, yet within each weekly session high performing learners are less tied to the nominal task order. We then model the sequences of high and low performance students using the probablistic Bayesian model and show that we can learn engagement behaviors associated with performance. We also show that the data sequence framework can be used for task-centric analysis; we identify critical junctures and differences among types of tasks within the course design. We find that non-rote learning tasks, such as interactive tasks or discussion posts, are correlated with higher performance. We discuss the application of such analytical techniques as an aid to course design, intervention, and student supervision.



<p align="center">
  <img src="/images/research/student_tasks.png" height="500px" width="500px" />
</p>


[Article](https://doi.org/10.1038/s41598-021-81709-3){: .btn--research} 




