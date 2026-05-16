---
layout: single
title: "Autonomous Racecar Software"
permalink: /projects/autonomous-racecar/
toc: true
toc_label: "Contents"
header:
  overlay_image: /assets/images/fs-italy-2025/fs-italy-2025-car-front.jpg
  overlay_filter: "0.35"
  caption: "Formula Student Italy 2025"
---

Software and systems work for a Formula Student Driverless racecar, spanning ROS 2 integration, localization, mapping, perception interfaces, and embedded deployment.

## Overview

This project covers the software stack around autonomous racing: turning sensor data into a usable vehicle state estimate, maintaining a map of the cone-defined track, and deploying the stack on embedded compute hardware under competition constraints.

{% include figure image_path="/assets/images/fs-italy-2025/fs-italy-2025-car-trackdrive.jpg" alt="Autonomous Formula Student racecar driving through cones at FS Italy 2025" caption="Track testing at Formula Student Italy 2025." %}

## Responsibilities

- ROS 2 software integration for autonomous racing workflows
- localization, mapping, and cone-based environment representation
- deployment and testing on NVIDIA Jetson-based compute
- Dockerized development and runtime environments
- event support during inspection, testing, and judging

## Competition Context

Formula Student events turn the software into a full systems problem: the car has to work with real sensors, real timing constraints, inspection procedures, changing track conditions, and short debugging windows.

{% include figure image_path="/assets/images/fs-italy-2025/fs-italy-2025-judging.jpg" alt="Technical judging discussion beside the Formula Student racecar at FS Italy 2025" caption="Technical judging and system discussion at FS Italy 2025." %}

## Testing

Track sessions are where the assumptions in simulation and log replay meet the actual vehicle. The software has to tolerate noisy detections, changing grip, sensor alignment issues, and practical operational constraints around staging and recovery.

{% include figure image_path="/assets/images/fs-italy-2025/fs-italy-2025-car-back.jpg" alt="Rear view of the autonomous Formula Student racecar aligned with cones" caption="Vehicle staged on a cone-defined course." %}

{% include figure image_path="/assets/images/fs-italy-2025/fs-italy-2025-rainy-ebstest.jpg" alt="Team member beside the autonomous racecar during rainy EBS testing" caption="Rainy test conditions during event operations." %}

## Technologies

ROS 2, C++, Python, NVIDIA Jetson, Docker, Linux, sensor integration, localization, mapping, and autonomous racing tooling.

## Event Media

{% include figure image_path="/assets/images/fs-italy-2025/fs-italy-2025-tirechange.jpg" alt="Team member working near the racecar tire at FS Italy 2025" caption="Pit and setup work around the vehicle." %}
