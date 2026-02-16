---
layout: project
title: "RoboCup Rescue Line"
description: "Develop line following robot"
description_long: "Develop line following robot at the Schülerforschungszetrum (SFZ) Südwürttemberg (student research center)."
date: 2018-02-25
categories: [Robotics, RPI, Mechatronics]
featured_image: "/assets/images/projects/sfz/featured.jpg"
#github_url: "https://github.com/yourusername/your-project"
#demo_url: "https://youtu.be/your-demo-video"
featured: true

gallery:
  - type: "image"
    file: "/assets/images/projects/sfz/board.jpg"
    description: "Own developed pcb"
  - type: "image"
    file: "/assets/images/projects/sfz/featured.jpg"
    description: "Finished robot"

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
  - name: "Drive chains"
    quantity: 2
    description: "Drive train"
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
#  - type: "video"
#    file: "/assets/images/projects/your-project/demo.mp4"
#    description: "Demo video description"
#  - type: "image"
#    file: "/assets/images/projects/your-project/demo.gif"
#    description: "Animated GIF demonstration"
---



## SFZ in general
The <a href="https://sfz-bw.de/" target="_blank">SFZ</a> is an extracurricular program for school students, where they can learn a wide range of knowledge-based MINT topics. Students can learn independently in groups with constant supervision. They can participate in projects such as programming, artificial intelligence (AI), robot programming, model aircraft, and game development. Alternatively, they can bring their own ideas to the free research topic.

## My discipline
Develop, build, and program a robot from scratch to compete in the Rescue Line discipline at the RoboCup Germany. In this competition, robots must follow a line with different obstacles and intersections. During the tournament, each group competes against the others and is ranked based on the robot's ability to complete the course.

## Technical Details
My group started with different starter kits for multiple years and decided to diverge from the mainstream concept of using nearly pre-built robots from LEGO, Fischertechnik, and other providers. We chose to start from scratch. We were aware of the challenges and poor performance in competitions, but considered them secondary to the learning and fun of building and failing. 

The robot's base, gripper, and structure were 3D-printed. The base components, such as the motors, chain drive, and display, were bought. We used C++ and git for the base development. We also used a camera with OpenCV for more advanced topics.

## Learnings
- [x] Work in a self organizing team
- [x] Lead and represent a team
- [x] Develop the hardware and software of a robot
- [x] Prioritize different development ideas
- [x] Participate in the competition
- [x] Organize sponsors and support for the team