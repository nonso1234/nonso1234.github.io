---
title: "ME 495 Sawyer Tic Tac Toe Project"
excerpt: "Sawyer Tic Tac Toe project site"
sidebar:
  - title: "Responsibilities"
    text: "Tic-tac-toe AI logic.  Connecting code between each main task"
gallery:
  - url: /assets/images/unsplash-gallery-image-1.jpg
    image_path: assets/images/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
  - url: /assets/images/unsplash-gallery-image-2.jpg
    image_path: assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
  - url: /assets/images/unsplash-gallery-image-3.jpg
    image_path: assets/images/unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 3"
---

The project task involved programming the Sawyer robotic arm to be able to play tic tac toe with a human player.  This involved 4 main tasks: computer vision, AI, motion planning, and force control.

<iframe width="560" height="315" src="https://www.youtube.com/embed/J4vcd4qHMO0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

- Computer vision was tasked for determining what the current state of the gameboard was and converting it to an array.  
- AI took that array and determined the cell coordinate that would provide the robot with the best next move.  
- Motion planning got the dry erase marker to the targeted cell, drew a shape, and returned to the camera configuration.  
- During motion planning, force feedback is control the Y coordinate of the dry erase marker.  If the marker is not being pressed hard enough on the whiteboard, the Y coordinate is lowered which applies more force.  If the marker is being pressed too hard, the Y coordinate is raised which reduces the applied force.
