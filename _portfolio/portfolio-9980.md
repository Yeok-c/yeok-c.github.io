---
title: "6 DOF Motion Simulator (2022)"
excerpt: "2nd Runner Up – EIE Microcontroller Application Design Competition 2022. <br/><img src='/images/portfolio/Cover_GIF.gif' width='600'>"
collection: portfolio
---


<div style="width:100%;text-align:center;">
<a href="https://github.com/Yeok-c/Stewart_Platform_Motion_Simulator"> <img src="/images/github-mark.png" width="100"> </a>
</div>

Deeply interested but lacking opportunities to work on robotic projects, I actively sought out opportunities for more practical experience on robotics. At the time, I had just completed [Dr. David Navarro-Alarcon](https://www.romi-lab.org/people)'s course on Perceptual Robotics. I have also conversed with fellow researchers from Professor Yick's team ([whos project went on to win Gold at Geneva Awards](https://www.polyu.edu.hk/media/media-releases/2023/0429_polyu-wins-record-breaking-number-of-awards-at-geneva-inventions-expo/)) on the motion simulation of realistic human-like movement. 

Feeling inspired, I studied - and wrote the [first python implementation of the inverse kinematic controller of Stewart Platforms](https://github.com/Yeok-c/Stewart_Py), the detailed explanation of which is available in [this Jupyter Notebook](https://github.com/Yeok-c/Stewart_Py/blob/main/01_Stewart_Py_Inverse_Kinematics.ipynb). I went head to go beyond the standard formulation of stewart platforms using linear actuators, and use rotational servos instead, which is considerably faster and more affordable, at the expense of analytical complexity. 

I then created a [small scale, proof-of-concept real world motion simulator](https://github.com/Yeok-c/Stewart_Platform_Motion_Simulator). I collected motion capture data, developed the controller, 3D CAD and prototyped a small mannequin that simulates movement of a human body based on the motion capture data. Here's a [demonstration of the prototype](https://connectpolyu-my.sharepoint.com/:v:/g/personal/18078696d_connect_polyu_hk/EfUZtXLRAtRKtvPQnRfG8H0BFq9Ugrqu71tGcmrLM1iN1g?e=bu1Euz). 

I eventually submitted this project to the "EIE Microcontroller Application Design Competition 2022", in which I received 2nd runner up. 

Presentation Video
<iframe width="560" height="315" src="https://www.youtube.com/embed/IOjBiIqHOO0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


<!-- 
<div style="max-width: 640px"><div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;"><iframe src="https://connectpolyu-my.sharepoint.com/personal/18078696d_connect_polyu_hk/_layouts/15/embed.aspx?UniqueId=d3cb53ba-de63-47a1-969b-34e0cd488206&embed=%7B%22ust%22%3Afalse%2C%22hv%22%3A%22CopyEmbedCode%22%7D&referrer=OneUpFileViewer&referrerScenario=EmbedDialog.Create" width="640" height="360" frameborder="0" scrolling="no" allowfullscreen title="Final_Presentation - Copy.mp4" style="border:none; position: absolute; top: 0; left: 0; right: 0; bottom: 0; height: 100%; max-width: 100%;"></iframe></div></div> -->

