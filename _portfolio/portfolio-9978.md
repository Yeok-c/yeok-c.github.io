---
title: "Research Assistant at Professor Joanne Yip's lab (2021-2022)"
excerpt: "Member of research team developing an AI-enabled biofeedback sportswear. <br/><img src='/images/portfolio/RA.png' width='600'>"
collection: portfolio
---

I have always been interested in the representational capabilities of learned models. I joined Dr. Joanne Yip’s multidisciplinary team as a research assistant to develop AI-enabled wearable sensors for sport science applications. Sports science is a difficult domain for predictive models, given the incredible inter-subject and inter-trial variability, the inherent lack of samples for critical events such as task failure, and the terrible signal-to-noise ratio due to sweat and movement artifacts. 

To pre-process the large, high-dimensional dataset (over 5TB) of surface electromyography (sEMG) and IMU signals collected from multiple sensors, I developed a lengthy semi-automated pipeline in MATLAB to perform:  
 - Data cleaning (remove empty sections, detect and remove corrupted data / disconnected sensors)
 - Pre-processing (bandpass filter, convert units)
 - Manipulation and rearrangement (label and rearrange channels for better readability)
 - Segmentation (segment cyclic motions, provide finer labels for concentric and eccentric segments in relevant exercises)

I later re-packaged all the scripts into a MATLAB application for future researchers' ease of use

<video src="/images/portfolio/RA.mp4" controls width="550" title="MATLAB Application for processing SEMG datasets"></video>

My familiarity with the sEMG data and machine learning techniques aided me in publishing a paper (first author) at the AHFE 2022 on our machine learning approach to predict muscle fatigue (link in publication page). To the best knowledge, we were the first to make predictions of muscle fatigue in real-time while the exercise set is incomplete without access to future data. In the project,
 - I communicated with our in-house sports scientist to develop suitable normalization methods that only utilize prior information within the same trial.
 - I designed the experiments and assisted other researchers in collecting over hundreds of samples across several participants
 - Our methods yield accuracy of 86% or f1-score of 0.624 for detecting muscle fatigue-induced task failure, impressive considering the rare nature of task failures. 

Conference presentation

<iframe width="560" height="315" src="https://www.youtube.com/embed/xfG4jmnyrAI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

The research findings, including the proposed novel normalization method, enabled me to then develop an end-to-end deep neural network to make predictions on muscle fatigue as a regression problem, integrating a deep convolutional neural network for sEMG waveforms and an embedding network that utilizes metadata (subject’s body composition, signal metadata, etc.).

Throughout the 15-month journey, I had many opportunities to apply technical knowledge gained from lectures in practice. I learnt a lot on research and experiment design, statistics for research and the academic world in general. On top of that, I learnt a lot on sports science from our in-house, licensed personal trainer (I gained over 8kg muscle over the year lol). Special thanks to my supervisor: Professor Joanne Yip, my mentors: Frances K.W. Wan and Alex Mak, my teammates and everyone at the lab who made journey a fun experience!


Other links
US Patent Application No. US20240001196A1, published at https://patents.google.com/patent/US20240001196A1 
CN Patent Application No. 202210781291.7 [Link](https://www.mtl-sft.com/patent/%E4%BA%BA%E5%B7%A5%E6%99%BA%E8%83%BD%E8%BC%94%E5%8A%A9%E5%80%8B%E4%BA%BA%E8%A8%93%E7%B7%B4%E7%B3%BB%E7%B5%B1%E3%80%81%E5%80%8B%E4%BA%BA%E8%A8%93%E7%B7%B4%E8%A3%9D%E7%BD%AE%E5%92%8C%E6%8E%A7%E5%88%B6/)
