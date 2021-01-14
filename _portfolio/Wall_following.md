---
title: "Mobile robotics maze solving using Wall following Algorithm"
header:
  teaser: "assets/images/mazefollower.png"
excerpt: "Mobile Robotics"
gallery:
  - url: /assets/images/unsplash-gallery-image-1.jpg 
    image_path: assets/images/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
---

<html>
<body>

<h1>Maze Solver Mobile robot on CoppeliaSim</h1>
I recently started working with CoppeliaSim software and I thought this would be a decent intro project. CoppeliaSim is a really cool simulation environment for quick robotic software testing in a near realistic environment. It provides a library of mobile robots (Holonomic and non-holonomic drives), manipulators and legged robots with some editable base code. Code is mostly written in Lua.

The goal of this project was to autonomously guide a robot through a maze course. I used a wall following algorithm to achieve this. I used an off-center kinematic control, which basically minimizes the positional and velocity error between an off center point and the center point of the robot, to compute joint velocities for the robot. More detailed explaination in the video below. I decided to use a lumibot differential drive mobile robot, adding proximity sensors on the left, right sides and front to get distance from the wall relative to the robot. To test the code, I started out with an easy maze. This maze course had gaps in between, and as a result, code generated errors whenever the proximity sensor distance data did not read float or integer values. Also, distance data were used in calculations, therefore nil values could not be used for running calculations. An easy fix was to substitute the max range of the sensor whenever the distance returned nil. However, this slightly affected the motion as you can tell from the video. The robot is programmed to keep at a defined distance from the wall throughout the course, therefore, whenever the proximity reads a higher or lower value, the robot adjusts to maintain this clearance (0.5 in this case)

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZwyNKNBrfM4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
I got the maze course from Dr Pranav Bhounsule's robotics course at UIC. 

Then I tried a more difficult maze, with 90 degree turns and curves. Also, fixed the jerky turns in the previous maze by breaking down different motion states (curve, turn, wall following, stop) and coded the kinematic equations in functions that return the joint velocities at the different states. This allowed for smoother state switching.  
<iframe width="560" height="315" src="https://www.youtube.com/embed/6yck7JEf_Hw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

Below is a video of a detailed explanation of an application of off-center kinematic control and wall following using a differential drive by Leopold Armesto. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/r03dFeZA2SY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

</body>
</html>