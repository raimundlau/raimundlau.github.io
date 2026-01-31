---
layout: project
title: "Drawing robot"
description: "Drawing an arbitrary .svg on a whiteboard."
description_long: "This project is about a lecture assignment to draw a arbitrary .svg file on a whitboard using an Universial Robot UR10e with a 3D printed Marker holder. It enables to safely operate a robot and teaches the basics of a Cobot."
date: 2025-11-17
categories: [Robotics, TUM]
featured_image: "/assets/images/projects/drawing_robot/featured.jpg"
github_url: "https://gitlab.lrz.de/tum-impl-ws25/group1/assignment-drawing/-/tree/master/student_work_group_01?ref_type=heads"
demo_url: "https://www.youtube.com/watch?v=UC3RvJ7HVww"
featured: true

# 3D Models
models:
  - file: "/assets/models/drawing_robot/model.gltf"
    description: "Used marker holder"

# Circuit Schematics
#schematics:
#  - file: "/assets/schematics/your-project/circuit.png"
#    description: "Your circuit description"



# Components List
components:
  - name: "UR10e"
    quantity: 1
    description: "Cobot"
    link: "https://www.universal-robots.com/"
  - name: "Whiteboard"
    quantity: 1
    description: "Whiteboard"
  - name: "Markerholder"
    quantity: 1
    description: "Markerholder as tool"

# Media gallery with images, videos, and GIFs
gallery:
  - type: "image"
    file: "/assets/images/projects/drawing_robot/setup.jpg"
    description: "Robot setup"
  - type: "image"
    file: "/assets/images/projects/drawing_robot/plane.jpg"
    description: "Plane teaching"
  - type: "image"
    file: "/assets/images/projects/drawing_robot/christmas_tree.jpg"
    description: "Christmas cards for family"
---



## Project goal
- Use a UR Cobot to teach the Tool Center Point of the marker holder tool and the drawing plane.
- Create a robot program to draw an arbitrary image at a predefined area of the whiteboard.


## Technical Details
For the Tool Center Point calibration we used the multi-pose-approach with the UR Pendant. The plane was also generated with the 3 point mehtod with the UR Pendant. The images at the right show the robot setup we worked with and the testin of the quality of the teached plane.

We used the simulation software [RoboDK](https://robodk.com/) to program the robot movements, simulate it for checking functionality and safety, and create the robot program, which is used on the real robot.

In the robot program the image file, the board and image size can be set, as well as the image position relative to the board. The reachability and a safety distance between image and the board border is automatically tested and set.

For an example usecase we drew christams cards for the family with different images. One example is shown at the right.


## Learnings
[x] Learn to safely handle and operate a robot
[x] Understand the principle of a Cobot
[x] Usage of software like RoboDK for robot simulation
[x] Transfer external programs to the robot
[x] teleoperate robot from Laptop