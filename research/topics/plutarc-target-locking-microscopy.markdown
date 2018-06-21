---
layout: researchtopic
title:  "PLuTARC: Target-Locking Microscopy"
lang: en
id: plutarc-target-locking-microscopy
permalink: /research/plutarc-target-locking-microscopy

description: Colloids are microscopic particles so small that they move diffusively when dispersed in a fluid, exhibiting Brownian motion, controlled by the temperature of the system, like atoms. However, unlike atoms, colloids are big enough to see with light, so they can be probed with microscopes and laser light scattering. 

thumbnail: PLuTARC_Cluster_480_thumbn.jpg

youtube_single: 
youtube_playlist: 

publications:
- OpEx_07
- Confocal_05
---
In any typical data gathering process, objects are observed from a fixed viewpoint (think of a camera on a tripod). If the objects are moving, this limits the observation time, as the objects move out of the field of view. In a microscope, this is a particularly severe problem when studying moving objects like swimming cells, or freely-diffusing cluster of colloidal beads. What we've done with the PLuTARC (Peter Lu Target-Locking Acquisition in Real-time Confocal) system is to implement target-locking. Images from the microscope are analyzed in real-time, allowing determination of the largest object's center. The automated microscope stage is then adjusted to keep that point centered in the 3D field of view. Then the next set of images is captured, and the stage moved once again. In this way, the motion of the object is physically subtracted from the measurement, so dynamic changes can be observed within the moving object for much longer than a simple static measurement. We've demonstrated this system’s capabilities by target-locking freely-diffusing clusters of attractive colloidal particles, and actively transported quantum dots (QDs) endocytosed into live cells free to move in three dimensions, for several hours. During this time, both the colloidal clusters and live cells move distances several times the length of the imaging volume. Watch the demo movie to see the system in action!

But the PLuTARC system's basic premise, integrating real-time geometric analysis of multiple objects into the image acquisition process, might also be more broadly applied with different imaging techniques. For instance, you might use the same ideas to steer an unmanned aerial vehicle tracking a migrating flock of birds for thousands of miles, well beyond the range of any static radar array. Or perhaps targeting tumors in parts of the body that move (due to breathing, for instance), in order to apply radiation treatment. We've filed a patent for some of these applications, and would be very interested in talking with you if you want to collaborate to actually build something cool!