---
layout: project
title: "Erasing robot"
description: "Erasing a defined on a whiteboard."
date: 2025-12-09
categories: [Robotics, TUM]
featured_image: "/assets/images/projects/erasing_robot/featured.jpg"
github_url: "https://gitlab.lrz.de/tum-impl-ws25/group1/assignment-erasing/-/tree/main/group1_erasing?ref_type=heads"
demo_url: "https://www.youtube.com/watch?v=jKivvzIEQQw"
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
components:
  - name: "Franka Research 3"
    quantity: 1
    description: "Cobot"
    link: "https://franka.de/de-de/products/franka-research-3"

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

Your project content goes here. Use Markdown for formatting.

## Project Overview
This assignment is about teaching a robot a motion along a surface and then execute this movement to erase a previously drawn image.
For that a Franka Research 3 robot is used holding a 3D printed tool, covered in cloth to clean and polish the drawing surface of a dry-erase whiteboard.

## Technical Details
Add technical specifications, algorithms, etc...