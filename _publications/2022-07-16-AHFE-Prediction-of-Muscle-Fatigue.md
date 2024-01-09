---
title: "Prediction of Muscle Fatigue During Dynamic Exercises based on Surface Electromyography Signals Using Gaussian Classifier"
collection: publications
permalink: /publication/2022-07-16-AHFE-Prediction-of-Muscle-Fatigue
excerpt: ''
date: 2022-07-16
venue: 'Applied Human Factors and Ergonomics International Conference'
paperurl: 'https://openaccess.cms-conferences.org/publications/book/978-1-958651-39-1/article/978-1-958651-39-1_8'
citation: 'Cheah, Y., Wan, K., Yip, J.  (2022). Prediction of Muscle Fatigue During Dynamic Exercises based on Surface Electromyography Signals Using Gaussian Classifier. In: Ravindra S. Goonetilleke and Shuping Xiong (eds) Physical Ergonomics and Human Factors. AHFE (2022) International Conference. AHFE Open Access, vol 63. AHFE International, USA.
http://doi.org/10.54941/ahfe1002597'
---


Abstract: Muscle fatigue is shown to be associated with incidence of musculoskeletal injuries found with sports training and competition. The real-time detection of fatigue onset allows preventative measures to be taken in time to minimize injuries. In this paper, we aim to provide a framework that classifies muscle fatigue based on surface electromyography (sEMG) features extracted during dynamic exercises. This includes the use of data segmentation, real-time-compatible data normalization, a principal component analysis (PCA) based feature reduction and Gaussian classifier methods.An experiment has been carried out to acquire the sEMG signals of the upper two pairs of rectus abdominis muscles of four healthy adult volunteers during weighted decline and bench-assisted sit-ups. The collected sEMG signals are then segmented into concentric and eccentric segments by using the inertial measurement unit (IMU) data. Eight commonly used sEMG features are extracted from each segment. We fit two Gaussian models (GMs) on the distribution of fatigued and non-fatigued data samples and show that the GM can utilize this information to predict the number of repetitions possible before task failure. We fit another set of GM on a reduced feature space by projecting the data onto principal component axes obtained through singular value decomposition (SVD). By projecting the features onto the first two principal axes, we achieve similar accuracy and f1-scores compared to the GM by using 6 handpicked features. This reduction in the feature space greatly reduces the training samples necessary for such class-imbalanced datasets. This classifier can also be directly used in the real-time detection of muscle fatigue during dynamic movements, which can be adopted in applications in sports, workplaces, and rehabilitation sciences. These frequency-time characteristics also provide insight into the function of low-level feature extractors when developing deep learning models to identify muscle fatigue.


Conference presentation

<iframe width="560" height="315" src="https://www.youtube.com/embed/xfG4jmnyrAI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


[Download paper here](http://yeok-c.github.io/files/2022-07-16-AHFE-Prediction-of-Muscle-Fatigue.pdf)

Link: https://openaccess.cms-conferences.org/publications/book/978-1-958651-39-1/article/978-1-958651-39-1_8