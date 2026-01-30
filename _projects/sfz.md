---
layout: project
title: "RoboCup Rescue Line"
description: "Schülerforschungszetrum Südwürttemberg"
date: 2018-02-25
categories: [Robotics, RPI, Mechatronics]
featured_image: "/assets/images/projects/sfz/featured.jpg"
#github_url: "https://github.com/yourusername/your-project"
#demo_url: "https://youtu.be/your-demo-video"
featured: false

# 3D Models
models:
  - file: "/assets/models/sfz/robot_base.gltf"
    description: "3D printed base of the robot"




# Components List
components:
  - name: "Raspberry Pi"
    quantity: 1
    description: "Main microcontroller"
    link: "https://www.raspberrypi.com/"
  - name: "Own developed boards"
    quantity: 2
    description: "e.g. interface and connection boards"
    #link: "https://www.raspberrypi.com/"
  - name: "Motor"
    quantity: 2
    description: "Drive train"
    #link: "https://www.raspberrypi.com/"
  - name: "Battery"
    quantity: 1
    description: "Power"
    #link: "https://www.raspberrypi.com/"
  - name: "Camera"
    quantity: 1
    description: "Raspberry Pi camera"
    link: "https://www.raspberrypi.com/"

# Media gallery with images, videos, and GIFs
#gallery:
#  - type: "image"
#    file: "/assets/images/projects/your-project/photo1.jpg"
#    description: "Project photo description"
#  - type: "video"
#    file: "/assets/images/projects/your-project/demo.mp4"
#    description: "Demo video description"
#  - type: "image"
#    file: "/assets/images/projects/your-project/demo.gif"
#    description: "Animated GIF demonstration"
---

# SFZ - Schülerforschungszentrum (student research centre)

## Project Overview
Develope, build, and program a robot from scratch to participate the RoboCup Germany in the discipline Rescue Line.

## Technical Details
The BerryBot group started with different starter kits for multiple years and decided to diverge from the mainstream concept of using nearly pre-built robots from LEGO, Fischertechnik, and other providers. We chose to start from scratch. We were aware of the challenges and poor performance in competitions, but considered them secondary to the learning and fun of building and failing.

The robot's base, gripper, and structure were 3D-printed. The base components, such as the motors, chain drive, and display, were bought. We developed the program from scratch in C++.