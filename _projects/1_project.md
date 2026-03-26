---
layout: page
title: "Spatial Perception & Registration"
description: Algorithmic foundations for spatial correspondence and deep learning-based medical image registration.
img: assets/img/NePhi_teaser.png
importance: 1
related_publications: true
---

Spatial perception is the foundation of spatial intelligence: before an AI system can understand or reason about anatomy, it must first estimate how structures correspond and deform across images and time.

My research develops the algorithmic foundations for spatial correspondence and alignment, including transformation regularization, similarity learning, and uncertainty estimation. These components form the infrastructure for building reliable and generalizable spatial models in medical imaging.


#### Transformation Regularization

I study how to represent and regularize deformation fields so that they are physically plausible, diffeomorphic, and generalizable across datasets and anatomies.

**GradICON** {% cite tian2023gradicon %} achieves state-of-the-art diffeomorphic registration via gradient inverse consistency regularization. 

**NePhi** {% cite tian2023nephi %} represents deformation fields as neural implicit functions for memory-efficient high-resolution registration. 

**CARL** {% cite greer2025carl %} introduces an equivariance framework for image registration.


#### Similarity Measure

I study how to measure anatomical similarity across images, especially across modalities where intensity values are not directly comparable.

**SAMConvex** {% cite li2023samconvex %} and **SAME++** {% cite tian2023samepp %} leverage self-supervised anatomical embeddings for fast and accurate cross modality registration.

#### Uncertainty Estimation

I study how to quantify the uncertainty of spatial correspondence, which is critical for clinical decision-making and downstream tasks.

I propose **test-time uncertainty estimation** {% cite tian2025uncertainty %} via transformation equivariance.

