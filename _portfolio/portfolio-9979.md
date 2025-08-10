---
title: "Modified Car Engine Recognition with Deep Neural Networks (2021-2022)"
excerpt: "Final Year Project: Modified Car Engine Recognition with Deep Neural Networks, under Professor Mak Man Wai<br/><img src='/images/portfolio/FYP_Cover.png' width='600'>"
collection: portfolio
---


<div style="width:100%;text-align:center;">
<a href="https://github.com/Yeok-c/Comparing-Acoustic-Deep-Neural-Networks"> <img src="/images/github-mark.png" width="100"></a>
</div>

## Project Video

<div style="width:100%;text-align:center;">
<iframe width="560" height="315" src="https://www.youtube.com/embed/YLQrOSpWTUQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

I conducted my Final Year Project (FYP) under [Professor Mak Man Wai](http://www.eie.polyu.edu.hk/~mwmak/), titled: Modified Car Engine Recognition with Deep Neural Networks. 

The goal of the project is to be able to accurately detect the presence of modified car engines in noisy urban environments. Many enthusiasts enjoy modifying their car engines for additional horsepower, certain effects or simply to sound more powerful. However, driving with unlicensed modifications on the highway may be dangerous, and is illegal in many places in the world. Furthermore, modified car engine sounds are also associated with illegal open-road racing activities (which are so popular in Malaysia they have a special term: 'Mat Rempit'). The goal is to train and deploy a deep-learning model to identify the sound profile (volume, timbre, pitch, and more abstract features) of modified engines, in the noisy backdrop of an urban environment. 

I approached the year-long project by performing an elaborate literature review, investigating various aspects of deep learning instead of focusing on the predictive model alone. I implmented the following and packaged it in my Github repo so running a bash script would install the packages, prepare the datasets, and run all the experiments.

- Dataset is downloaded, normalized, resampled and manually verified, from:
  - Audi Car Engine Database
  - Environmental Sound Classification-50
  - UrbanSounds8K
  - Audioset
  - Self-curated Youtube Videos of Modified Cars and Engines Sounds. 

- Data augmentation methods: MixUp and SpecAugment

- Different SOTA model architectures, including
  - MobileNetV1 (YAMNET, transfer learned)
  - MobileNetV2
  - MobileNetV3
  - VGG16 (VGGish, transfer learned)
  - EfficientNetv1B0
  - EfficientNetV2B0
  - Conv Mixer

- Evaluation method: K-fold (K=10) training and evaluation 

- Hyperparameter tuning: SK-Learn

- Visualization: Layer activation visualization, real-time inference and prediction visualization. 

My enthusiasm for the topic ensured A+ and a Technical Excellence Award (Top 3 in the program) on the Final Year Project, and A+, A+ and A on the three mentioned technical electives. 