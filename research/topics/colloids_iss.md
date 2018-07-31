---
layout: researchtopic
title:  "Colloids on the Space Station"
lang: en
id: colloids_iss
permalink: /research/colloids_iss
description: "Under normal conditions on earth, the separation between liquids and gases is usually a bit mundane: the level of water in a drinking glass simply falls as the liquid evaporates into a gas, since the liquid is denser."

youtube_single: 
youtube_playlist: 

thumbnail: Phase_separation_grid_040706_thumb.jpg

publications:
- JRTIP_09
links:
- <a href="http://science.nasa.gov/headlines/y2004/16jun_colloids.htm?list914346" target="_blank">Science@NASA</a> (Jun 2004)
---
Under normal conditions on earth, the separation between liquids and gases is usually a bit mundane: the level of water in a drinking glass simply falls as the liquid evaporates into a gas, since the liquid is denser. Two liquids of different densities, such as the oil and vinegar of salad dressing, are similarly unexciting; the oil just floats to the top after a period of time. However, when the effects of gravity are taken away, such as in the environment of the International Space Station (ISS), this separation creates far more interesting and complex patterns.

We have created mixtures of colloidal particles and polymers that separate into liquid and gas phases over the course of several days on ISS, and using time-lapse photography we are able to watch the changes in these samples and the patterns they form. Specifically, we examine a type of phase separation called spinodal decomposition near the critical point, a set of specific conditions where the properties of liquids and gases are the same. To do these experiments, we work closely with astronauts in orbit aboard the ISS, and some of our recorded conversations are in the player.

To analyze the data, we implement image correlation, a fundamental component of many real-time imaging and tracking systems, on a graphics processing unit (GPU) using NVIDIAs CUDA. We use our code to analyze images of liquid-gas phase separation in a model colloid-polymer system, photographed in the absence of gravity aboard the International Space Station (ISS). Our GPU code is 4000 times faster than simple MATLAB code performing the same calculation on a central processing unit (CPU), 130 times faster than simple C code, and 30 times faster than optimized C++ code using single-instruction, multiple data (SIMD) extensions. The speed increases from these parallel algorithms enable us to analyze images downlinked from the ISS in a rapid fashion and send feedback to astronauts on orbit while the experiments are still being run.
