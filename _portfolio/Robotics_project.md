---
title: "Robotics LARPA Project Challenge"
header:
  teaser: "assets/images/Robotics_LEGO.jpg"
excerpt: "Robotics Course final project"
sidebar:
   - title: "Responsibilities"
     text: "Gripper pick and place code in MATLAB. Identify and fix bugs in code" 
gallery:
  - url: /assets/images/unsplash-gallery-image-1.jpg 
    image_path: assets/images/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
---

<html>
<body>

<h1>LEGO Automated Reliable Powered Agents (LARPA) Robotics Challenge</h1>
<p>
This challenge mimicked the DARPA Robotics challenge 2015. Each team had to create an autonomous robotic system using a LEGO Mindstorm EV3 kit. The robot is required to autonomously perform a series of tasks along a course before exiting. Breakdown of the tasks as shown: 

<ul>
  <li>Task 1 : Debris Clearing</li>
  <li>Task 2: Park on blue patch for a specfic amount of time</li>
  <li>Task 3: Pick control rod (Aluminum can) from designated location </li>
  <li> Task 4: Navigate through narrow brigde </li>
  <li> Task 5: Place control rod in yellow patch</li>
  <li>Task 6: Exit Course </li>
</ul>  
Our robot was a simple two wheeled differential drive robot. We used the available sensors provided in the LEGO kit - Ultrasonic for distance measurement, Color sensor to identify colors, Gyro sensor to measure orientation in degrees. 

Overall all tasks had to be performed in under 120 secs. It helped that the course was color coded so we took advantage of this to localize and perform certain tasks. Code was written in MATLAB. 

Below is a video of the debris clearing task 
<iframe width="560" height="315" src="https://www.youtube.com/embed/qQem7EBzldo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</p>

</body>
</html>










