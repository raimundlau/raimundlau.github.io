---
layout: project
title: "Taskboard manipulation"
description: "Manipulate a taskboard with a cobot"
description_long: "This project is a lecture assignment about manipulating an electronic task board built for benchmarking robot manipulation. The focus is on automatically detecting and precisely controlling the cobot."
date: 2026-01-26
categories: [Robotics, TUM, IMPL]
featured_image: "/assets/images/projects/taskboard/featured.jpg"
github_url: "https://gitlab.lrz.de/tum-impl-ws25/group1/assignment-task-board/-/tree/main/group1_task-board?ref_type=heads"
#demo_url: "https://www.youtube.com/watch?v=UC3RvJ7HVww"
featured: true

# 3D Models
#models:
#  - file: "/assets/models/drawing_robot/model.gltf"
#    description: "Used marker holder"

# Circuit Schematics
#schematics:
#  - file: "/assets/schematics/your-project/circuit.png"
#    description: "Your circuit description"



# Components List
#components:
#  - name: "Franka Research 3"
#    quantity: 1
#    description: "Cobot"
#    link: "https://franka.de/de-de/products/franka-research-3"

# Media gallery with images, videos, and GIFs
gallery:
  - type: "image"
    file: "/assets/images/projects/taskboard/featured.jpg"
    description: "Robot setup"
  - type: "image"
    file: "/assets/images/projects/taskboard/detection.jpg"
    description: "Detection from taskboard and buttons"
---

## Project Goals
- Detect and classifiy parts on the electronic [taskboard](https://github.com/peterso/robotlearningblock)
- Move the robot with ROS to the detected objects
- Manipulate the taskboard with a robot

## Technical Details
The [taskboard](https://github.com/peterso/robotlearningblock) is an electronic real-world benchmarking platform for evaluating robot manipulation skills. The box has different modules which focuses on different manipulation skills. For this project the Find-, speed-, and light-test were used.

The perception task uses image and depth information gathered by a RealSense camera. The 3D coordinates of the box and both buttons are calculated and transformed into the correct coordinate frames. Then, the robot can move to these coordinates and interact with the box.

The logic for perception and task completion is written in ROS packages with connections to existing Franka packages.

## Learnings
- [x] Learn robot manipulation capabilities
- [x] Perception tasks with RGBD camera
- [x] Computer vision tasks with image- and depth data
- [x] Transformations between different robot frames