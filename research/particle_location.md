---
layout: researchtopic
title:  "Fast, Accurate Particle Location"
lang: en
id: particle_location
permalink: /research/particle_location
areas: high_performance_imaging, soft_matter_physics

description: High-performance imaging software and methods to determine rapidly and precisely the 3D positions of many colloidal particles in microscope images.

thumbnail: PLuTARC_Cluster_480_thumbn.jpg

youtube_single: mZm6I5j_bq0
youtube_playlist: 

publications:
- OpEx_07
- OpEx_13
- PhDThesis_08
- Confocal_05
---
We present a number of methods to locate, rapidly and accurately, fluorescent particles imaged with fluorescence and confocal microscopy. 

We have implemented the traditional Crocker and Grier methodology to locate particles, with accelerated CPU and GPU libraries. As a result, the particle detection is sufficiently fast and accurate to be fed back into the mechanical control of a microscope stage, enabling real-time target-locking of colloidal clusters, as shown in the video. Because we can follow a growing colloidal cluster as it moves out of the original fixed field of view, we can extend significantly the observation time of these processes, beyond the limits that diffusion typically imposes. We have also been able to observe actively-transported quantum dots (QDs) endocytosed into live cells free to move in three dimensions, for several hours. 

We have also looked carefully at all of the stages of these algorithms, and show that accurately locating particles in 3D requires circular convolution kernels, not the square kernels chosen in earlier implementations for performance reasons. While seemingly a trivial detail, in fact using non-circular kernels can lead to the artifactual detection of crystallinity in dense, disordered particle suspensions that do not in reality have significant crystalline order.
