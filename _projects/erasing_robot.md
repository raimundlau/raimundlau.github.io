---
layout: project
title: "Erasing robot"
description: "Erasing a defined area on a whiteboard with a cobot"
description_long: "This project is about a lecture assignment to erase a text on a whitboard using an Franka Emika Research 3 Cobot. This project focuses on the different controllers and kinematics from robots."
date: 2025-12-09
categories: [Robotics, TUM]
featured_image: "/assets/images/projects/erasing_robot/featured.jpg"
github_url: "https://gitlab.lrz.de/tum-impl-ws25/group1/assignment-erasing/-/tree/main/group1_erasing?ref_type=heads"
demo_url: "https://www.youtube.com/watch?v=jKivvzIEQQw"
featured: true


# Components List
#components:
#  - name: "Franka Research 3"
#    quantity: 1
#    description: "Cobot"
#    link: "https://franka.de/de-de/products/franka-research-3"

# Media gallery with images, videos, and GIFs
gallery:
  - type: "image"
    file: "/assets/images/projects/erasing_robot/setup.jpg"
    description: "Robot setup"
  - type: "image"
    file: "/assets/images/projects/erasing_robot/training.jpg"
    description: "Area teaching without tool"
  - type: "image"
    file: "/assets/images/projects/erasing_robot/erasing.jpg"
    description: "Testing the erasing"
---

## Project Goals
- Teach the FR3 cobot a motion along a surface.
- Replay this movement with enough force against the whiteboard
- Erase previously drawn image of a dry-erase whitboard


## Technical Details
This project uses ROS2 to control the robot and an interactive terminal to guide users through the workflow. The robot can be used in two modes. 

In teaching mode, the absolute joint positions and time relative to the starting time are saved. In this mode, the operator moves the robot arm over the whiteboard to record the erasing movement, as shown in the second picture.

In erasing mode, the robot, with an erasing tool attached, replays the recorded movements while taking the realtive time into account to achieve the teached velocity.

The robot's controller is programmed to allow slight deviations in the path to smooth out the teaching movements and improve the erasing quality.


## Learnings
- [x] Control a cobot with ROS2
- [x] Teach and replay movements
- [x] Compare and customize controller for the usecase
- [x] Force-controlled movements for cobot