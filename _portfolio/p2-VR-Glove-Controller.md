---
title: "VR Glove Controller Winter Project 2020"
header:
  teaser: "assets/images/vrglove.jpg"
excerpt: "VR Glove project site"
gallery:
  - url: /assets/images/unsplash-gallery-image-1.jpg
    image_path: assets/images/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
---

[VR Glove Github Repo](https://github.com/bespeland/vr-glove)

This project's goal was to design and build a virtual reality controller that could accurately track finger movements beyond the what is currently offered in commercial virtual reality controllers (most use buttons with capacitive sensing).  The method used to detect finger bend are flex sensors attached to a glove.  The following is a demonstration of me bending my fingers while wearing the glove and a 3D hand model in Unity moving to match.  

<iframe width="560" height="315" src="https://www.youtube.com/embed/ef_XSX4a4gE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


This does not entail any computer vision (which is how finger tracking is typically implemented in virtual reality with devices such as the LeapMotion). The flex sensors bend with my finger and I can measure how much each sensor is bending.  I feed this data back into my computer to be interpreted by Unity to move the hand model.  
